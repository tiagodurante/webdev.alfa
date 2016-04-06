# Audio no HTML5

Agora, no HTML5, existe a possibilidade de reproduzir audio de determinanos formatos sem a necessidade de um plugin específico (Microsoft ou Adobe). A novidade pode ser executada em qualquer navegador que ja tenha suporte.

Browser | MP3 | WAV | OGG
------- | --- | --- | ----
Internet Explorer | SIM | NÃO | NÃO
Google Chrome | SIM | SIM | SIM
Firefox | SIM (Versão 21 ou superior no Windows 7, 8, Vista e Android) | SIM | SIM
Safari | SIM | SIM | NÃO
Opera | NÃO | SIM | SIM

### MIME-type

O MIME-type é o recurso que determina qual o tipo de dado será processado logo em seguida. No caso do áudio, são estes:

Formato | MIME-type
------- | ---
MP3 | audio/mpeg
OGG | audio/ogg
WAV | audio/wav

### Atributos

* **controls** : exibe os controles de play/pause, volume e tempo de execução do audio;
* **autoplay** : o audio é executado logo que a página é carregada;
* **loop** : faz com que o audio continue em execução, mesmo que termine;
* **muted** : carrega o audio com o audio mutado;
* **preload** : exibe informações do autor sobre o vídeo durante o carregamento da página;
* **src** : diretório do audio

```html
<audio autoplay controls loop>
	<source src="audio.ogv" type="audio/ogg">
	<source src="audio.mp3" type="audio/mp3">
	<strong>Atenção:</strong> Seu navegador não possui suporte a HTML5
</audio>
```
