# How to install My Arr Stack

You will need to create a compose.yml and have docker run it. This should also work in GUI's like dockage, Portaioner, etc.

## Installation

Before you install you will need to edit the location for where you want the volumes 

```yml
volumes:
      - [insert file path here]/Prowlarr:/config
      - [insert file path here]/Media/:/media
```

You will need to change this and it should auto create if path is not already made.
