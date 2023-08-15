
---
<div style="background-image: url(https://media3.giphy.com/media/wwg1suUiTbCY8H8vIA/giphy.gif?cid=ecf05e47hfu84pmh8vk2mo5wohm7vxo4hcx1gu3ye1664zcy&ep=v1_gifs_search&rid=giphy.gif&ct=g); display: flex; justify-content: center;">

# Sicer Andres Brito Gutierrez 🧑‍💻 Documentación Comandos Publicos 📖
</div>


<div style="display: flex; justify-content: center;">

## Documentación de varios comandos de herramientas y lenguajes de programación hecha por [Sicer Brito 🧑‍💻](https://github.com/SicerBrito)
</div>




## Índice 📑

- [Documentación 📖](#documentación)
    - [NetCore](#netcore) <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ee/.NET_Core_Logo.svg/2048px-.NET_Core_Logo.svg.png" width="10px">
        - [Descripción](#descripción)
        - [Instalación](#instalación)
            - [Actualización del Sistema](#actualización-del-sistema)
            - [Instalación de Dependencias](#instalación-de-dependencias)
            - [Agregar Repositorio de Microsoft](#agregar-repositorio-de-microsoft)
            - [Instalación de NetCore](#instalación-de-netcore)
            - [Verificación](#verificación)
        - [Comandos Basicos](#comandos-basicos)
            - [Estructura Base](#estructura-base-🚧)
            - [Referencias](#referencias-🔗)
        - [Gestión de Datos](#gestión-de-datos-🧑‍💻)
            - [Instalacion de Paquetes](#instalacion-de-paquetes-🔧)
            - [Migrations](#migrations-✈️)


## Documentación

### NetCore

- ### Descripción
    .NET y .NET Core son dos plataformas de desarrollo de software desarrolladas por Microsoft, .NET Framework es la plataforma de desarrollo tradicional de Microsoft para aplicaciones Windows, mientras que .NET Core es su contraparte moderna y multiplataforma.

    .NET Core es una plataforma de desarrollo de software de código abierto y multiplataforma que Microsoft creó para abordar las limitaciones del .NET Framework y permitir el desarrollo de aplicaciones tanto en Windows como en otros sistemas operativos, como Linux y macOS. <img src="https://www.emojiall.com/images/animations/joypixels/64px/writing_hand.gif" width="35">

- ### Instalación
    - ### Actualización del Sistema:
        Abre una terminal y ejecuta los siguientes comandos para asegurarte de que el sistema esté actualizado ✅

            sudo apt update
            sudo apt upgrade

    - ### Instalación de Dependencias
        Asegúrate de tener las dependencias necesarias instaladas. En Ubuntu, puedes hacerlo con el siguiente comando ✅

            sudo apt install curl libunwind8 gettext apt-transport-https

    - ### Agregar Repositorio de Microsoft
        Agrega el repositorio de Microsoft para .NET Core ✅

            curl -fsSL https://packages.microsoft.com/keys/microsoft.asc | sudo gpg --dearmor -o /usr/share/keyrings/microsoft-archive-keyring.gpg

            echo "deb [arch=amd64 signed-by=/usr/share/keyrings/microsoft-archive-keyring.gpg] https://packages.microsoft.com/repos/microsoft-ubuntu-22.04.3 LTS-prod focal main" | sudo tee /etc/apt/sources.list.d/microsoft.list

        Reemplaza "22.04.3 LTS" con el nombre de la versión de Ubuntu que estés utilizando si es diferente

    - ### Instalación de NetCore 
        Actualiza los paquetes e instala .NET Core ✅

            sudo apt update
            sudo apt install dotnet-sdk-7.0

        Cambia 7.0 por la versión de .NET Core que quieras instalar.

    - ### Verificación

        Verifica que .NET Core se haya instalado correctamente ✅

            dotnet --version

<img src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200908124347/Differences-Between-.NET-Core-and-.NET-Framework.png" width="3000px">

 - ### Comandos Basicos
    ---
        dotnet new
        
    Crea un nuevo proyecto o archivo basado en una plantilla. Puedes usarlo para crear aplicaciones de consola, aplicaciones web, bibliotecas y más.

    Ejemplo: dotnet new console -n MiProyecto

    ---
        dotnet build

    Compila un proyecto y sus dependencias. Genera los archivos binarios y los coloca en la carpeta de salida.

    Ejemplo: dotnet build

    ---
        dotnet run

    Compila y ejecuta un proyecto en una sola acción. Es útil para probar rápidamente una aplicación.

    Ejemplo: dotnet run

    ---
        dotnet publish
    Publica una aplicación para su implementación. Esto compila y empaqueta la aplicación para que pueda ser ejecutada en un entorno específico.

    Ejemplo: dotnet publish -c Release -o MiPublicacion

    ---
        dotnet restore
    Restaura las dependencias de un proyecto. Descarga los paquetes NuGet especificados en el archivo .csproj.

    Ejemplo: dotnet restore

    ---
        dotnet test
    Ejecuta las pruebas unitarias en un proyecto. Busca y ejecuta las pruebas definidas en el proyecto.

    Ejemplo: dotnet test

    ---
        dotnet clean
    Limpia los archivos generados por la compilación, como los binarios y los archivos intermedios.

    Ejemplo: dotnet clean

    ---
        dotnet new solution
    Crea una nueva solución que puede contener varios proyectos. Es útil para organizar proyectos relacionados.

    Ejemplo: dotnet new solution -n MiSolucion

    ---
        dotnet sln
    Gestiona soluciones que contienen múltiples proyectos. Puedes agregar, quitar o listar proyectos en la solución.

    Ejemplo: dotnet sln MiSolucion.sln add MiProyecto/MiProyecto.csproj

    ---
        dotnet add
    Agrega referencias o proyectos a una solución o a un proyecto.

    Ejemplo: dotnet add MiProyecto/MiProyecto.csproj reference OtraBiblioteca/OtraBiblioteca.csproj

    ---
        dotnet new web
    Crea un nuevo proyecto de aplicación web ASP.NET Core.

    Ejemplo: dotnet new web -n MiAplicacionWeb

    ---
