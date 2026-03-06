# Meeskonnaliikmed:
    Ilmar Murakas
    Krete Kivit
    Martin Kilp

# Serverivariant:
    Zone.ee
        * tasuta .eu lõpuga domeen
        * Kooli poolt  aasta tasuta domeen + server
        * head manualid githubiga integreerimiseks (pipeline)
  
# Serveriinfo:
    * 217.146.69.57
    * ZoneOS | Release 25.09.00
    * Apache

# SSH:
    Kokku 4 võtit millest kolm public keyd läksid zones ssh seadistuse alla + private key läks githubi secret alla.

    * ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIDSbb+6uHFLnYA6KKiFzEochvGLqlkFSadnI7K5chT3k krete@krete
    * ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIAThp4j2/z9CsNqaA2VdL9K1ZD++iDXurMbxmLKg7FsH ilmar@ilmar
    * ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAILYZmaaZO/8oWIzqQPtakveNefaaxn3qdHZDB+X++ZFl marti@MaKiLap

    github secrets:
        * SSH_HOST = 217.146.69.57
        * SSH_USER = virt145947
        * DEPLOY_PATH = /data01/virt145947/domeenid/www.martinkilp.eu/htdocs
        * SSH_PRIVATE_KEY = salajane
  
  # Probleemid:
    *ssh võtmepaaride genereerimisel salvestas terminal valesse asukohta. Pidime pc useri juur kausta .ssh/ kausta genereerima. - chatgpt abiga saime korda.
    * githubis repode jagamine + õiguste andmine (Collaborators) - ghatgpt abiga saime korda.
    * github action secrets lisasime kõik 4 secretit ühte kogumisse, tegelt peavad kõik eraldi olema. - chatgpt abiga saime korda.
  
  # Deploy testmise tulemus:
    tegime ühe branchi (main) ja pushisime ühte branchi.
    kõikidel deploy õnnestus.
    


