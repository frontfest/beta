# FrontFest 2020

Web para la cuarta edición de FrontFest.

## Instalación

Esta web funciona con Jekyll, con lo cual es necesario tener previamente instalado el entorno de [Ruby](https://www.ruby-lang.org/es/) y el gestor de dependencias [Bundler](https://bundler.io/).

- Instalamos Ruby:

```
sudo apt install ruby-full
```

- Instalamos Bundler:

```
sudo gem install bundler
```

## Ejecución en local

- Instalamos las dependencias de la web. Se almacenarán en el directorio *vendor*.

```
bundle install
```

- Levantamos la web:

```
bundle exec jekyll serve
```

Y accedemos desde el navegador a http://localhost:4000
