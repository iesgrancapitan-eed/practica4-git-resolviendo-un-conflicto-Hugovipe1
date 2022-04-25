1. Asegúrate de que tienes configurado el editor Visual Studio Code como tu editor de Git. (git config --global core.editor "code --wait")

    ![Editor](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.01.07.png)

2. Crea un repositorio local y avanza en la rama "master" añadiendo un fichero "index.html" con la estructura básica html. El body estará vacío

    ![GitInit](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2019.57.07.png)

    ![GitCommit](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2019.58.51.png)
3. Crea y salta a "rama-1". Avanza en un commit con tu nombre de pila en un párrafo dentro del body

    ![gitBranch](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.03.48.png)
    ![GitCommit](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.07.44.png)
4. Vuelve a la rama master

    ![GitCheckout](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.09.46.png)
5. Crea y salta a "rama-2". Avanza en un commit con tu apellido en un párrafo dentro del body

    ![GitBranch](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.11.04.png)
    ![GitImage](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.14.06.png)
6. Muestra el estado del repositorio de forma gráfica y resumida

    ![GitLog](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.18.58.png)
7. Haz un merge a rama-1. Intentas fusionar ambas ramas. Aparecerá un conflicto porque ambos commits trabajan en la misma porción <body></body> de un mismo archivo index.html. Git no será capaz de fusionarlas directamente.

    ![GitMerge](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.20.41.png)

8. El editor VS Code reconoce los conflictos de fusión. Las diferencias se resaltan y hay acciones en línea para aceptar los cambios. Deja un único párrafo con tu nombre de pila y apellido.

    ![Editor](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.22.33.png)
9.  Una vez que se resuelto el conflicto confirma el archivo en conflicto para que pueda realizar esos cambios

    ![GitCommit](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.37.19.png)
10. Muestra de nuevo el estado del repositorio de forma gráfica y resumida
    
    ![ModoGráfico](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.41.24.png)
11. Vuelve a la rama master y realiza otro merge. Es una fusión fast-forward. Los dos commits a fusionar tienen relación de ancestro. Entonces el merge no produce un commit nuevo, sencillamente avanza la rama, "avance rápido"

    ![GitCheckoutGitMerge](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.44.47.png)
12. Visualiza las ramas que han sido fusionadas con la rama master

    ![GitBranch](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.46.21.png)
13. Elimina las ramas correctamente fusionadas (sin asterisco) para quedarte SOLO con la rama master.
    ![GitBranch](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.49.24.png)

14. Realiza una copia a este repositorio remoto

    ![GitRemote](image/Captura%20de%20pantalla%202022-04-25%20a%20las%2020.53.24.png)
15. Recuerda añadir estas instrucciones con los pantallazos en el fichero README.md
16. En GitHub entra en Insights/network y visualiza el gráfico del repositorio con los merge y cinco commits  1. 