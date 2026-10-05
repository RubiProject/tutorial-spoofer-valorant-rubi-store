# 3-flash-bios

> For the complete documentation index, see [llms.txt](https://private-store.gitbook.io/tutorial-spoofer-valorant-private-store/llms.txt). Markdown versions of documentation pages are available by appending `.md` to page URLs; this page is available as [Markdown](https://private-store.gitbook.io/tutorial-spoofer-valorant-private-store/2-configuracao/flash-bios.md).

## Flash Bios

Etapas OBRIGATÓRIAS para todas as placas-mãe

{% hint style="info" %}
**Aviso:** A atualização incorreta do BIOS pode danificar seu sistema. Prossiga por sua conta e risco. Certifique-se de ter a versão correta do BIOS e uma fonte de alimentação estável. Peça ajuda ao suporte, se necessário!
{% endhint %}

**Identificando sua placa-mãe** e informações do sistema

1. Informações do sistema aberto (msinfo32 na barra de pesquisa)
2. Encontre <mark style="color:orange;">o produto e o fabricante da BaseBoard.</mark>
3. Nota <mark style="color:red;">Versão/Data da Bios</mark>

{% hint style="warning" %}
<mark style="color:$info;">\*\*Observação: se as informações do seu sistema estiverem imprecisas ou forem incertas, acesse as configurações de UEFI/BIOS e verifique as informações.\*\*</mark>
{% endhint %}

**TUTORIAL PARA CADA PLACA-MÃE**

{% tabs %}
{% tab title="ASUS" %}
**PRIMEIRO** , baixe e execute esta ferramenta[ferramenta](https://mega.nz/file/gtRVEQDT#5hHDR00CGiBPRDfLlPtlU21o7jJBrLOCPp3ka7llark)

**OPÇÃO 1**

* Certifique-se de baixar uma versão da Bios diferente da atual (de preferência, faça o downgrade de uma versão)
* Formate seu USB para FAT32. (Clique com o botão direito do mouse em USB, clique em formatar, coloque FAT32 no sistema de arquivos) Se o seu USB não tiver a opção FAT32, use esta ferramenta: [**CLIQUE EM MIM**](https://www.majorgeeks.com/mg/getmirror/fat32format,1.html)

**OPÇÃO 2**

* Não esqueça de baixar a versão da Bios de 2021/2020.
* Formate seu USB para FAT32. (Clique com o botão direito do mouse em USB, clique em formatar, coloque FAT32 no sistema de arquivos) Se o seu USB não tiver a opção FAT32, use esta ferramenta: [**CLIQUE EM MIM**](https://www.majorgeeks.com/mg/getmirror/fat32format,1.html)

Tutorial aqui 👇
{% endtab %}

{% tab title="MSI" %}
* Certifique-se de baixar uma versão da Bios diferente da atual (de preferência, faça o downgrade de uma versão)
* Formate seu USB para FAT32. (Clique com o botão direito do mouse em USB, clique em formatar, coloque FAT32 no sistema de arquivos) Se o seu USB não tiver a opção FAT32, use esta ferramenta: [**CLIQUE AQUI**](https://www.majorgeeks.com/mg/getmirror/fat32format,1.html)
* **Tutorial** 👇
{% endtab %}

{% tab title="GIGABYTE" %}
* Certifique-se de baixar uma versão da Bios diferente da atual (de preferência, faça o downgrade de uma versão)
* Formate seu USB para FAT32. (Clique com o botão direito do mouse em USB, clique em formatar e coloque FAT32 em Sistema de Arquivos) Se o seu USB não tiver a opção FAT32, use esta ferramenta: [**CLIQUE** ](https://www.majorgeeks.com/mg/getmirror/fat32format,1.html)AQUI

**Tutorial** 👇
{% endtab %}

{% tab title="ASROCK" %}
* Certifique-se de baixar uma versão da Bios diferente da atual (de preferência, faça o downgrade de uma versão)
* Formate seu USB para FAT32. (Clique com o botão direito do mouse em USB, clique em formatar, coloque FAT32 no sistema de arquivos) Se o seu USB não tiver a opção FAT32, use esta ferramenta: [**CLIQUE AQUI**](https://www.majorgeeks.com/mg/getmirror/fat32format,1.html)

**Tutorial** 👇
{% endtab %}
{% endtabs %}

**Habilitar TPM**

1. Habilite o TPM (Suporte a Dispositivos de Segurança) na **aba Segurança do BIOS (Trusted Computing)**
2. Se você tiver uma CPU AMD, habilite também **o fTPM**

{% tabs %}
{% tab title="INTEL" %}
**Desabilite estas opções listadas abaixo**

Desabilitar CSM

Desabilitar FAST BOOT
{% endtab %}

{% tab title="AMD" %}
**Desabilite estas opções listadas abaixo**

Desabilitar CSM

Desabilitar FAST BOOT
{% endtab %}
{% endtabs %}

**Habilitar inicialização segura**

1. Habilite a inicialização segura na **guia de inicialização do BIOS - Restaurar chaves de inicialização de fábrica**

**Ativar o HVCI (ISOLAMENTO DE NUCLEO)**

**Confirme as configurações corretas**

1. No Windows, pesquise por **msinfo32** e pressione Enter. Verifique se o valor para **Estado de Inicialização Segura** está **Ativado.**
2. Procure por **tpm.msc** e pressione Enter. Deverá aparecer a mensagem **"O TPM está presente".**
