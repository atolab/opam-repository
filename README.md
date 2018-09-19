# ATOLab Opam Repository
This is the opam repository that hosts all the open source OCaml packages developed by ADLINK's Advanced Technolgy Office. 

# Configuring the ATO Repository
The first thing to do is check the repository you have already configured. To do so execute the command:

    $ opam repository list --all
  
Assuming that the **atolab** repository does not appears on the list already than do the following to add it:

    $ opam repository add atolab git+https://github.com/atolab/opam-repository.git  
    $ opam update

# Testing the ATO repository
To test if the **atolab** opam repository has been correctly added do:

    $ opam info apero-net
  
You should get the following result:

    <><> apero-net: information on all versions <><><><><><><><><><><><><><><><><><>
    name         apero-net
    all-versions 0.3.0

    <><> Version-specific details <><><><><><><><><><><><><><><><><><><><><><><><><>
    version       0.3.0
    repository    atolab
    url.src:      "https://github.com/atolab/apero-net/archive/v0.3.0.tar.gz"
    url.checksum: "md5=94ced95cae33e9a2e12f9dc933fb51fc"
    homepage:     "https://github.com/atolab"
    bug-reports:  "https://github.com/atolab/apero-net/issues/"
    dev-repo:     "git://github.com/atolab/apero-net.git"
    authors:      "Angelo Corsaro"
    maintainer:   "angelo@adlink-labs.tech"
    license:      "Apache-2.0"
    depends:      "dune"
                  "cmdliner"
                  "fmt"
                  "logs"
                  "lwt"
                  "ppx_deriving"
                  "uuidm"
                  "yojson"
                  "lwt_ppx"
                  "apero-core" {>= "0.3.0"}
    synopsis      OCaml Networking Library
    description   apero-net is collection of OCaml libraries that simplify the task of writing
                  network protocol and network services.
