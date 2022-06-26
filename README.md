# MoveBalls

> Version 2

Ejercicio de la semana 2 con el propósito de controlar el DOM desde javascript así como controlar diferentes arrays en tiempo de ejecución.


## Resultado

https://user-images.githubusercontent.com/106959153/175811982-3840a961-4fb4-494f-8302-e2501b55497f.mp4

## Highlights

El uso de forEach [^1] en un array:

´´´
  balls.forEach (element => {
      calcNewPosition(element);
      let currentBall = document.getElementById(element.name);
      currentBall.style.left = element.left + 'px';
      currentBall.style.top = element.top + 'px';    
    }
  )
´´´


## Versioning

Releases will be numbered with the following format:

`<major>.<minor>.<patch>`

**The major version "2" is part of an umbrella release.  It includes many different types of files and technologies. Therefore
we deviate from normal SemVer in the following ways:**

* Any release may update the design, look-and-feel, or branding of an existing
  icon
* We will never intentionally release a `patch` version update that breaks
  backward compatibility
* A `minor` release **may include backward-incompatible changes** but we will
  write clear upgrading instructions in UPGRADING.md
* A `minor` or `patch` release will never remove icons
* Bug fixes will be addressed as `patch` releases unless they include backward
  incompatibility then they will be `minor` releases


[^1]: https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
