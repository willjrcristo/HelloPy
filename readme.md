´´ Install ``

Link para download do instalador do Python
https://www.python.org/ftp/python/3.12.1/python-3.12.1-amd64.exe

Link para download do instalador do Git
https://objects.githubusercontent.com/github-production-release-asset-2e65be/23216272/255edd25-cca0-4294-909c-b46bced63e3f?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20230913%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230913T131733Z&X-Amz-Expires=300&X-Amz-Signature=c7305a41775e250241e8a66153febfaee4bb76b38cf5e4a5ad995e6de06fff65&X-Amz-SignedHeaders=host&actor_id=0&key_id=0&repo_id=23216272&response-content-disposition=attachment%3B%20filename%3DGit-2.42.0.2-64-bit.exe&response-content-type=application%2Foctet-stream

Link para download do instalador do VSCode
https://objects.githubusercontent.com/github-production-release-asset-2e65be/23216272/255edd25-cca0-4294-909c-b46bced63e3f?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20230913%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230913T131733Z&X-Amz-Expires=300&X-Amz-Signature=c7305a41775e250241e8a66153febfaee4bb76b38cf5e4a5ad995e6de06fff65&X-Amz-SignedHeaders=host&actor_id=0&key_id=0&repo_id=23216272&response-content-disposition=attachment%3B%20filename%3DGit-2.42.0.2-64-bit.exe&response-content-type=application%2Foctet-stream

<h1>Passos usados na criação do projeto</h1>

Abri o Windows Explorer, naveguei até a área de trabalho e criei uma pasta chamada Py, dentro dela criei uma pasta chamada HelloPy

Então abri minha conta do Git e criei o repositório, então configurei minha pasta da seguinte forma:

Na barra de endereço do explorer, escrevi cmd e na janela do terminal:
git init
git remote add origin https://github.com/willjrcristo/HelloPy.git

Em seguida dei o comando "code ." para abrir o VSCode nessa pasta

Então criei o arquivo main.py e coloquei uma linha simples, printando uma mensagem, só pra constatar que o ambiente está funcional:

Abri o terminal dentro do vscode com Ctrl + ' (apóstrofo) e digitei:
python main.py

A mensagem apareceu no terminal!

Escrevi esse passo a passo e agora vou dar o commit inicial do projeto.

Depois vou encontrar um mote para o projeto, algo que o python seja particularmente bom, como IoT por exemplo.. Veremos..

``` Commit Inicial ```

No terminal do VSCode dei os comandos do git (já tive algumas bizarrices com UI do Git, mais especificamente SourceTree, e a gente não fica tão dependente de ferramentas de terceiros, embora eu use bastante o plugin do próprio vscode :)

git status
git add .
git commit -m "Texto explicativo"

É bom manter uma disciplina de commitar sempre que tiver algum avanço importante, criar branchs de feature quando for começar alguma tarefa, pois normalmente essa tarefa requer vários passos, e a cada passo, um commit.

E para subir as alterações, git push, mas no primeiro o git pede para adicionar o --set-upstream origin master (provavelmente porque eu não havia feito checkout na branch, apenas joguei os arquivos lá, comitei e fui empurrando... Mas aí o git pede para você explicitar pra onde você quer subir, no meu caso, por ser um commit inicial, vai na master mesmo.. Mas em um ambiente a vera, provavelmente haverá a necessidade de fazer Pull Request usando uma branch intermediária, pra ficar mais fácil de desfazer caso algo dê errado com esse novo código que está subindo)