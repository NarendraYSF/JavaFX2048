# JavaFX 2048 Game

JavaFX 2048 is a classic puzzle game implemented in Java using the JavaFX framework. The objective is to combine tiles with the same number to reach the 2048 tile.
![JavaFX 2048 Demo](https://github.com/NarendraYSF/JavaFX2048/blob/main/Demo2048Shot.png?raw=true)

## License

This project is licensed under the **GNU GENERAL PUBLIC LICENSE**. See the [LICENSE](https://github.com/NarendraYSF/JavaFX2048/blob/main/LICENSE) file for details.

## How to Clone the Repository

To clone this repository, use the following command in your terminal:

```bash
git clone https://github.com/NarendraYSF/javaFX2048.git
```

## How to Run the Program

To run the program, you will need to have **Gradle** installed. You can use `gradlew`, which is included in the repository. Follow these steps:

1. **Navigate to the project directory:**

    ```bash
    cd JavaFX2048
    ```

2. **Use the following command to run the application:**

    ```bash
    ./gradlew run
    ```

   This command will compile and execute the JavaFX application.

## Additional Information

- Ensure you have **JDK 11 or higher** installed on your machine.
- For building a distribution package, you can run:

    ```bash
    ./gradlew dist
    ```

- To create a native installer, use:

    ```bash
    ./gradlew jpackage
    ```

## Running using Docker
You can build container image from source code using the Dockerfile and run the containerized game. 
You have to share the X11 socket with the container. For that you need to install [VcXsrv Windows X Server](https://sourceforge.net/projects/vcxsrv/) for windows or [Xquartz](https://www.xquartz.org) if you're using macOS. Make sure to allow connections from network during setup.
On macOS, you'll need to run `xhost +127.0.0.1` every time you re-open Xquartz.
The final step is to run the container: `docker run -it --rm -e DISPLAY=host.docker.internal:0.0 image_name`

## Feedback / Contributing / Comments
Submit an issue and share your thoughts.
