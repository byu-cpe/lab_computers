1. Install Ubuntu 22

1. Install packages
    ```
    sudo apt update

    sudo apt install -y \
        build-essential \
        qtbase5-dev \
        clang-format-12 \
        zip \
        python3-pip \
        x11-apps \
        gcc-arm-none-eabi \
        python3-serial \
        xterm \
        openocd \
        python3-dev \
        python3-venv \
        valgrind \
        firefox \
        cmake
    ```

1. Test your cmake version, and make sure it is at least 3.14.5:
    ```
    cmake --version
    ```

1. Install VS Code <https://code.visualstudio.com/>



