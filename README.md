# thezoo_dockerized
Dockerized image of thezoo live malware repository

TheZoo: https://github.com/ytisf/theZoo
zoo script : https://github.com/Odyssey2247/thezoo_dockerized

INSTALL

    git clone https://github.com/Odyssey2247/thezoo_dockerized
    chmod +x zoo
    cp zoo ~/.local/bin //make sure it is in your PATH
    zoo

zoo install docker image if is not present

RUN
in terminal:

    $zoo

zoo conect docker container via ssh and ejecute thezoo
defaul credentials:

    USER: thezoo
    PASSWORD: thezoo

DOCKER RUN
for run thezoo witout the zoo script, run in terminal:

    docker pull jluis2247/thezoo
    docker run -d --name thezoo -p 2222:22 jluis2247/thezoo /usr/sbin/sshd -D
    ssh -t thezoo@127.0.0.1 -p 2222 'zoo'
