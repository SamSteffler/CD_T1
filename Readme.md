# Instruções de Execução - Visualizador de Códigos de Linha

##  Códigos Implementados

A ferramenta contempla todos os códigos base vistos em aula, além dos três códigos extras determinados pelo nosso grupo:

**Códigos Base:**
* NRZ-L e NRZ-I
* Manchester e Manchester Diferencial
* AMI e Pseudoternário

**Códigos Extras:**
* **MLT-3** (Multi-Level Transmit 3)
* **2B1Q** (2 Binary, 1 Quaternary)
* **CMI** (Coded Mark Inversion)


##  Como Executar a Ferramenta

A interface foi projetada para ser intuitiva e permitir a comparação direta entre diferentes esquemas de codificação em tempo real. Ela pode ser acessada diretamente pela [GitHub Pages](https://samsteffler.github.io/CD_T1/) do projeto ou abrindo o arquivo ```index.html``` em qualquer navegador.

### 1. Entrada da Sequência Binária
No topo da página, tem o campo de Entrada. Ali você pode digitar manualmente a sequência de bits que quer analisar. O campo possui validação e processa apenas os caracteres `0` e `1`. A atualização do gráfico ocorre em tempo real conforme a entrada digitada.

### 2. Escolha e Comparação de Códigos
Logo abaixo do campo de entrada, há uma barra com botões representando os códigos de linha implementados.

Basta clicar no código de linha que você quer ver a sequência de bits que ele ficará marcado e será exibido abaixo. Podem ser escolhidos todos os códigos de linha simultaneamente.

Os gráficos ficarão um embaixo do outro, permitindo comparar visualmente o comportamento da mesma sequência de bits em diferentes esquemas. Para remover um gráfico, basta clicar novamente no botão correspondente para desativá-lo.

### 3. Análise dos Gráficos e Métricas
Para cada código ativado, será renderizado um bloco contendo:
* **O Gráfico de Onda :** Com linhas de grade demarcando os intervalos de bit (ou pares de bits).
* **Painel de Propriedades:** Exibindo características teóricas relevantes do código, referentes aos problemas comuns de sincronização, componente DC e nível médio, nesse caso sobre afastamento da origem. Além disso, também exibe a banda teórica consumida e se o código de linha tem detecção de erro
* **Métricas:** Como pedido na atividade, ele mostra a quantidade de transições e o nível médio para a sequência de bits de entrada, calculados em tempo real com base na sequência de entrada fornecida.

### 4. Sobre a ferramenta
A ferramenta foi criada como uma página em HTML. As funções executadas para gerar o gráfico de onda, calcular o nível de tensão médio e o número de transições foram desenvolvidos em JavaScript. Para mais detalhes sobre o funcionamento de cada codificação, basta olhar as funções para a codificação desejada e os seus respectivos comentários. A estilização da página foi realizada com CSS embutido.

---
*Trabalho desenvolvido para a disciplina de Comunicação de Dados - UFSM (2026).*

*De autoria dos alunos Enzo Santin da Silveira, Luan Tiago Streck, Samuel Steffler e Tiago Steffler*
