## EN

### Setting up a simple Phishing Attack using <a href="https://github.com/trustedsec/social-engineer-toolkit"> Social-Engineer Toolkit </a>

<p>This documentation is part of a DIO Cyber Security bootcamp project and is available for educational purposes only, not being meant to be used for doing harm to others or for any illegal practice.</p>

<p>This challenge was conducted on a Kali Linux Virtual Machine. Although this is a simple process and could be done using your own operational system, start using virtualization and Kali Linux is interesting for those involved with cyber security studying, because Kali OS provides lots of pentesting and attacking tools (including SE Toolkit), while virtualization allows the creations of a sandbox/laboratory for cyber security studying, testing and exploring. Therefore, it is recommended to choose a virtualization software like VirtualBox or UTM (for Macs, especially ARM based) and create a Kali Linux virtual machine (search for "how to create a kali linux virtual machine using virtual box/utm")</p>

#### 1 - Go to root
<p>Inside Kali Linux, open the terminal and run '''sudo su''' to go to the root user. Insert the password for the root user.</p>

#### 2 - Start SE Toolkit
<p>Invoke SE Toolkit: '''setoolkit'''</p>

#### 3 - Social-Engineering Attacks
<p>From the menu, choose "Social-Engineering Attacks"</p>

#### 4 - Website Attack Vectors
<p>Choose "Website Attack Vectors"

#### 5 - Credential Harvester Attack Method
<p>Choose "Credential Harvester Attack Method"</p>

#### 6 - Site Cloner
<p>Choose "Site Cloner"</p>

#### 7 - Confirm host IP Address
<p>Press Enter/Return to confirm the host IP Address to be used</p>

#### 8 - Enter the URL to clone
<p>The URL provided must be complete, including "http://", for example: "https://www.facebook.com/"</p>

<p>A server with the cloned page will be set up in the address of the host IP (step 7) and can be accessed through the browser. The credentials passed to the phishing page should appear in the SE Toolkit report and the fake server should then redirect the victim to the real Facebook page, masking the scam. Nevertheless, modern browsers should efficiently block the request through CORS (Cross-Origin Resource Sharing) security machanism. Though, it actually worked (the passed credentials arrived to SET report) when I tested using Internet Explorer on a Windows 7 VM to access the server.</p>

<img width="400" alt="Facebook phishing server running on IE on a Windows 7 VM" src="./imgs/facebook_phishing.png">
<img width="400" alt="Credentials from phishing passed to SET Report" src="./imgs/credentials_passed.png">

## PT - BR

### Configurando um Ataque de Phishing Simples usando o <a href="https://github.com/trustedsec/social-engineer-toolkit">Social-Engineer Toolkit</a>

<p>Esta documentação faz parte de um projeto de um bootcamp de Cibersegurança da DIO e está disponível apenas para fins educacionais, não devendo ser usada para práticas maldosas ou ilegais.</p>

<p>Este desafio foi realizado em uma máquina virtual com o sistema operacional Kali Linux. Apesar de ser um processo simples que poderia ser feito em seu próprio sistema operacional, começar a utilizar virtualização e o Kali Linux é interessante para quem está estudando cibersegurança, pois o Kali OS oferece diversas ferramentas de pentest e ataque (incluindo o SE Toolkit), enquanto a virtualização permite a criação de um sandbox/laboratório para estudos, testes e exploração em cibersegurança. Portanto, recomenda-se escolher um software de virtualização, como VirtualBox ou UTM (para Macs, especialmente os baseados em ARM), e criar uma máquina virtual com o Kali Linux (procure por "como criar uma máquina virtual do Kali Linux usando VirtualBox/UTM").</p>

#### 1 - Acesse o usuário root
<p>No Kali Linux, abra o terminal e execute o comando '''sudo su''' para acessar o usuário root. Insira a senha do usuário root.</p>

#### 2 - Inicie o SE Toolkit
<p>Invoque o SE Toolkit: '''setoolkit'''</p>

#### 3 - Ataques de Engenharia Social
<p>No menu, escolha "Social-Engineering Attacks".</p>

#### 4 - Vetores de Ataque em Sites
<p>Escolha "Website Attack Vectors".</p>

#### 5 - Método de Captura de Credenciais
<p>Escolha "Credential Harvester Attack Method".</p>

#### 6 - Clonador de Sites
<p>Escolha "Site Cloner".</p>

#### 7 - Confirme o endereço IP do host
<p>Pressione Enter/Return para confirmar o endereço IP do host a ser utilizado.</p>

#### 8 - Insira a URL a ser clonada
<p>A URL fornecida deve estar completa, incluindo "http://", por exemplo: "https://www.facebook.com/".</p>

<p>Um servidor com a página clonada será configurado no endereço do IP do host (passo 7) e poderá ser acessado pelo navegador. As credenciais inseridas na página de phishing devem aparecer no relatório do SE Toolkit, e o servidor falso deve então redirecionar a vítima para a página real do Facebook, mascarando o golpe. No entanto, navegadores modernos devem bloquear a solicitação de forma eficiente por meio do mecanismo de segurança CORS (Cross-Origin Resource Sharing). Entretanto, funcionou (as credenciais chegaram ao relatório do SET) quando testei usando o Internet Explorer em uma máquina virtual com Windows 7 para acessar o servidor.</p>

<img width="400" alt="Servidor do Phishing do Facebook rodando no endereço host no IE em uma VM de Windows 7" src="./imgs/facebook_phishing.png">
<img width="400" alt="Credenciais coletadas através do phishing passadas ao relatório SET" src="./imgs/credentials_passed.png">
