# Vídeo no HTML5

Agora, no HTML5, existe a possibilidade de reproduzir audio de determinanos formatos sem a necessidade de um plugin específico (Microsoft ou Adobe). A novidade pode ser executada em qualquer navegador que ja tenha suporte.

Browser | MP4 | WEBM | OGG
------- | --- | --- | ----
Internet Explorer | SIM | NÃO | NÃO
Google Chrome | SIM | SIM | SIM
Firefox | SIM (Versão 21 ou superior no Windows 7, 8, Vista e Android) | SIM | SIM
Safari | SIM | NÃO | NÃO
Opera | NÃO | SIM | SIM

### MIME-type

O MIME-type é o recurso que determina qual o tipo de dado será processado logo em seguida. No caso do vídeo, são estes:

Formato | MIME-type
------- | ---
MP4 | video/mp4
WEBM | video/webm
WAV | video/ogg

### Atributos

* **controls** : exibe os controles de play/pause, volume e tempo de execução do vídeo;
* **autoplay** : o vídeo é executado logo que a página é carregada;
* **loop** : faz com que o vídeo continue em execução, mesmo que termine;
* **muted** : carrega o vídeo com o vídeo mutado;
* **preload** : exibe informações do autor sobre o vídeo durante o carregamento da página;
* **src** : diretório do vídeo;
* **poster** : exibe determinada imagem enquanto o vídeo é carregado;
* **width** : especifica a largura do player;
* **height** : especifica a altura do player;

```HTML5
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```
