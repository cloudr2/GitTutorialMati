# GitTutorialMati
Tutorial para que mati aprenda a usar GIT

Video de ayuda: https://www.youtube.com/watch?v=0fKg7e37bQE

1. Crear cuenta en https://github.com/
2. Instalar GIT en PC.
3. Configurar GIT local con GitHub.
4. Clonar proyecto.

## Modificar el Readme.md ##

1. Crear un branch desde el branch 'master', llamado 'develop'.
  * $ git checkout -b develop
2. Crear un branch desde el branch 'develop', llamado 'feature/tutorial_1'
  * $ git checkout -b feature/tutorial_1
3. Modificar el archivo README.MD, debajo del titulo 'Tutotial 1' agregando una linea por debajo que diga 'Completé el tutorial 1'.
4. Subir los cambios al branch remoto 'feature/tutorial_1'
  1. Revisar los cambios nuevos que estamos tratando de agregar.
    * $ git status
  2. Agregar los cambios a nuestro branch de 'feature/tutorial_1'
    * Agregar nuestro archivo modificado.
      * $ git add. readme.md
    * Subir los cambios a nuestro repositiorio local.
      * $ git commit -m "Modificacion del readme para tutorial."
  3. Revisar que nuestro branch troncal 'develop' esté actualizado.
    * Cambiar de branch 'feature/tutorial_1' a 'develop'
      * $ git checkout develop
    * Traer cambios (de existir) desde el repositorio remoto a nuestro repositorio local.
      * $ git pull origin develop
  4. Actualizar nuestro branch local 'feature/tutorial_1' con 'develop'.
    * Cambiar de branch 'develop' a 'feature/tutorial_1'.
      * $ git checkout feature/tutorial_1
    * Combinar los cambios del branch develop' con lo que tenemos en 'feature/tutorial_1' para asegurarnos que ambas versiones sean las mismas.
      * $ git merge develop
    * Subir la version definitiva de nuestra feature (cambios en el readme.md) al repositiorio remoto 'feature/tutorial_1'.
      * $ git push origin feature/tutorial_1
  5. Actulizar develop con nuetra ultima feature
    * Cambiar de branch 'feature/tutorial_1' a 'develop'.
      * $ git checkout develop
    * Revisar nuevamente que no haya cambios en 'develop'.
      * $ git pull origin develop
    * Combinar nuestra feature con el branch 'develop' para concluir el cambio.
      * $ git merge origin feature/tutorial_1
    * Subir los cambios al repositorio remoto 'develop'.
      * $ git push origin develop
      
   6. Ingresar a github.com y revisar que tanto en 'develop' como en 'feature/tutorial_1' el readme.md contenga la linea 'Completé el tutorial 1' debajo del titulo 'Tutotial 1'.
   
   ## Tutotial 1 ##
    
    
    
