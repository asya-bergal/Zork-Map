Dependies: GraphViz

The easiest way to add to the map in realtime is to set up a script that listens for modifications to map.dot, then automatically regenerates the image. To do so in Bash:

- Download `sleep_until_modified.sh` from [here]
- In Bash, run `while sleep_until_modified.sh map.dot; do dot map.dot -Tpng -o map.png; done`


[here]:https://bitbucket.org/denilsonsa/small_scripts/src/9159fee62dc7cca7f81f47cef41bd9ae1324553e/sleep_until_modified.sh?at=default
