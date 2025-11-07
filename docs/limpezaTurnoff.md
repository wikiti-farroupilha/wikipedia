PASSO A PASSO PARA INCLUIR O SCRIPT DE LIMPEZA DOS ARQUIVOS DOS USUÁRIOS NO WINDOWS


- Primeiramente crie uma pasta no C:\ chamada Scripts
- Insira nesta pasta o arquivo de PowerShell [LimparPerfilUsuario.ps1](https://drive.google.com/file/d/1tN1yplTaVJlSLTaPMwcRj50FXkzJMipb/view?usp=sharing) que encontra-se no nosso drive DTI na pasta Script limpeza usuário
- Entre no gpedit.msc como administrador
- No lado esquerdo da da janela vá em configuração do computador
- Acesse configuração do windows 
- Acesse Scripts(Inicialização/Encerramento)
- No lado direito da janela, de um duplo clique no desligamento
- Na janela que abriu, na aba Scripts, clique em Adicionar…
- No campo nome do Script digite: powershell.exe
- No campo Parâmetros de Script digite: - NoProfile -ExecutionPolicy Bypass -File “C:\Scripts\LimparPerfilUsuario.ps1”
- Clique em Ok
- Clique em Aplicar e depois em OK.
- Pronto está inclusa a rotina de limpeza quando o computador for desligado.
