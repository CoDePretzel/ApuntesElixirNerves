Para construir sistemas integrados con elixir 

¿Qué es Elixir?

Lenguaje de programación funcional con capacidad de meta-programinación

puedes desarrollar aplicaciones distribuidas 

¿Cómo Instalar Elixir?

Ir a la ruta https://elixir-lang.org/install.html y descarga dependiendo de tu sistema operativo.

Para windows es sencillo al ejecutar el archivo dar siguiente siguiente hasta finalizar

Si estas usando otro sistema operativo, sigue las instrucciones de la guía.

como comprobar que fue instalado, abrir un consola o terminal 
e ingresar 

~~~cmd
elixir --version
~~~

Si la salida es
~~~cmd
Erlang/OTP 24 [erts-12.1.5] [source] [64-bit] [smp:4:4] [ds:4:4:10] [async-threads:1] [jit]

Elixir 1.13.2 (compiled with Erlang/OTP 22)
~~~

También se puede instalar mediante docker.

Existen dos proyectos 

https://www.grisp.org/
https://www.nerves-project.org/

podemos instalar 
mediante la guía https://hexdocs.pm/nerves/installation.html

o mediante docker
https://github.com/NervesJP/docker-nerves

~~~bash
docker pull nervesjp/nerves
~~~

~~~bash
docker run -it -w /workspace nervesjp/nerves
~~~

¿Qué es Nerves?

Un framework para contruir sistemas integrados sobre elixir

Nerves es una completa plataforma e infraestructura de IoT para construir y desplegar sistemas embebidos mantenibles.

A buildroot-based infrastructure to cross compile extremely lean linux images that boot right into BEAM, ans start Elixir code in seconds.

Libraries, in Elixir, that target the core needs of embedded systems incluiding IO,networking firmware updates device discovery etc

Tooling to create and manage embedded systems


Raspberry Pi 
Beaglebone

Crear una nueva APP de Nerves

~~~
mix nerves.new hello_nerves
~~~