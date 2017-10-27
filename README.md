## overview

Custom ubuntu-based docker images with my own dotfiles etc.

I mainly use them combined with the following bash/zsh functions:

```
u14() {
    if [ ! -z $1 ]
    then
        echo $@
        docker run --rm $@ -it u14:latest
    else
        docker run --rm -it u14:latest
    fi
}

u16() {
    if [ ! -z $1 ]
    then
        echo $@
        docker run --rm $@ -it u16:latest
    else
        docker run --rm -it u16:latest
    fi
}

```
