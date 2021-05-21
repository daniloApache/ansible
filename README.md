<h1 align="center">
    <a href="http://ansible-br.org/">Ansible</a>
</h1>
<p align="center"> Repositório destinado a criar uma base de conhecimento com exemplos que possam ser reutilizáveis</p>

<h4 align="center"> 
	🚧  Repositório em contrução  🚧
</h4>

_______________________________________________________________________________________


<h2 align="left"> 
	Instalação Ansible
</h2>

1) Primeiro, atualize o cache do repositório de pacotes DNF com o seguinte comando:

$ sudo dnf makecache

2) Agora, para habilitar o repositório EPEL, instale o pacote epel-release com o seguinte comando:

$ sudo dnf install epel-release -y

3) Agora, atualize o cache do repositório de pacotes DNF novamente com o seguinte comando:

$ sudo dnf makecache

4) Instale o ansible

$ sudo dnf install ansible -y

5) Valide a instalação com o seguinte comando

$ ansible --version


<h2 align="left"> 
	Gerar o par de chaves SSH
</h2>

$ ssh-keygen

$ ssh-copy-id -i /root/.ssh/id_rsa.pub <usuário_node_destino>@<ip_ou_host_node_destino>

Realize o teste de acesso SSH.

$ ssh -i /root/.ssh/id_rsa.pub <usuário_node_destino>@<ip_ou_host_node_destino>
