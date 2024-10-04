# Atividade 1
# Trecho 1
We see three critical differences between programming and software engineering: time, scale, and the trade-offs at play. On a software engineering project, engineers need to be more concerned with the passage of time and the eventual need for change. In a software engineering organization, we need to be more concerned about scale and efficiency, both for the software we produce as well as for the organization that is producing it. Finally, as software engineers, we are asked to make more complex decisions with higher-stakes outcomes, often based on imprecise estimates of time and growth.

## Comentário
A engenharia de software deve ser muito mais flexível e adaptável do que a programação, devido à necessidade de considerar o tempo, que pode demandar mudanças futuras. Além disso, a preocupação com a escala e a eficiência é essencial para garantir a qualidade tanto do software produzido quanto da organização que o desenvolve. Por fim, os trade-offs envolvem tomadas de decisões mais complexas e resultados de maior impacto, frequentemente baseados em estimativas imprecisas de tempo e crescimento.

# Trecho 2
Within Google, we sometimes say, “Software engineering is programming integrated over time.” Programming is certainly a significant part of software engineering: after all, programming is how you generate new software in the first place. If you accept this distinction, it also becomes clear that we might need to delineate between programming tasks (development) and software engineering tasks (development, modification, maintenance). The addition of time adds an important new dimension to programming. Cubes aren’t squares, distance isn’t velocity. Software engineering isn’t programming.

## Comentário
A programação é uma parte essencial da engenharia de software, mas quando reconhecemos as distinções entre essas duas áreas e destacamos as tarefas específicas de cada uma, percebemos que a programação por si só não consegue suprir todas as demandas da engenharia de software. Da mesma forma, a engenharia de software não pode cumprir seu papel sem a programação. A frase “Software engineering is programming integrated over time.” captura essa diferença fundamental, ressaltando que a engenharia de software adiciona a dimensão do tempo à programação, transformando-a em um processo mais completo e contínuo.

# Atividade 2
# Analisando Ferramentas e comparando seus aspectos não funcionais:
Para uma melhor analise, eu destaquei seis aspectos de cada uma das comparações.

## React Native vs Flutter
Essas duas tecnologias populares para para o desenvolvimento de aplicativos móveis multiplataforma possuem algumas distinções, como:

**Performance:** O React Native pode ter performance limitada devido ao uso de uma bridge para comunicação entre o código JavaScript e os componentes nativos, o que pode introduzir overhead. Ele é geralmente adequado para a maioria dos aplicativos, mas não é tão eficiente quanto soluções nativas, especialmente em aplicações que exigem alta performance. Em contrapartida, Flutter compila diretamente para código nativo, oferecendo uma performance superior, especialmente em animações complexas e interfaces de usuário mais sofisticadas.

**Tempo de Desenvolvimento:** React Native se destaca pela grande quantidade de bibliotecas e componentes prontos, acelerando o desenvolvimento. Além disso, desenvolvedores familiarizados com JavaScript geralmente encontram facilidade em aprender e utilizar a tecnologia, reduzindo o tempo de integração. Flutter, apesar de exigir aprendizado da linguagem Dart, proporciona uma experiência de desenvolvimento eficiente com ferramentas como "hot reload", o que pode compensar o tempo inicial de aprendizado.

**Manutenibilidade:** O código em React Native pode ser mais fragmentado, especialmente em projetos maiores que envolvem código JavaScript, nativo e específico para Android e iOS, o que torna a manutenção mais desafiadora. Por outro lado, o código em Flutter tende a ser mais unificado, já que a interface do usuário e a lógica são escritas em uma única linguagem (Dart), facilitando a manutenção a longo prazo.

**Comunidade e Suporte:** React Native possui uma comunidade vasta e madura, com uma ampla gama de bibliotecas e recursos disponíveis, o que é uma grande vantagem na hora de buscar suporte. Flutter, embora ainda esteja crescendo, conta com suporte oficial do Google e uma comunidade em rápida expansão, o que indica um futuro promissor.

**Tamanho do Aplicativo:** Em geral, aplicativos React Native tendem a ser menores em comparação aos desenvolvidos com Flutter, o que pode ser uma vantagem para usuários com limitações de armazenamento. Aplicativos Flutter costumam ser maiores devido à inclusão da engine Flutter e das bibliotecas padrão.

**Suporte a Dispositivos e Plataforma:** React Native oferece bom suporte para Android e iOS, mas a adaptação para novas plataformas, como desktop, pode exigir trabalho adicional e bibliotecas de terceiros. Flutter, por sua vez, suporta Android, iOS, Web e está expandindo seu suporte para desktop (Windows, macOS, Linux), tornando-o uma opção mais versátil para aplicações multiplataforma.

## Kubernetes vs Docker Swarm
Agora vamos comparar tecnologias utilizadas para orquestração de contêineres, utilizando cinco aspectos principais:

**Escalabilidade:** O Kubernetes é altamente scalável, projetado para gerenciar milhares de contêineres distribuídos em vários nós. Adequado para grandes empresas e sistemas complexos que exigem escalabilidade massiva. Enaquanto o Docker Swarm oferece escalabilidade, mas em uma escala menor em comparação ao Kubernetes. É mais adequado para projetos de pequena a média escala.

**Complexidade de Configuração:** O Docker Swarm é bem mais fácil de configurar e iniciar, com uma curva de aprendizado menos acentuada. Ele se integra bem com Docker, o que torna a transição para a orquestração relativamente simples. Já o Kubernetes é conhecido por sua complexidade inicial de configuração. A curva de aprendizado é mais íngreme devido à sua ampla gama de funcionalidades e à necessidade de configurar diversos componentes (como networking, armazenamento, segurança).

**Resiliência e Recuperação de Falhas:** O Kubernetes é demasiadamente resiliente, com capacidade avançada de auto-recuperação e balanceamento de carga. Ele pode redistribuir cargas automaticamente em caso de falhas nos nós. O outro também oferece resiliência, mas em um nível inferior ao Kubernetes. Sua capacidade de recuperação de falhas é menos robusta.

**Comunidade e Suporte:** O Kubernetes possui uma das maiores e mais ativas comunidades no espaço de orquestração de contêineres, com suporte extenso e constante evolução. Já o Docker Swarm possui uma menor comunidade e menor foco no desenvolvimento, especialmente à medida que o Kubernetes se torna a escolha padrão para muitas organizações.

**Gerenciamento e Monitoramento:** O Docker Swarm possui ferramentas de gerenciamento e monitoramento mais limitadas, mas que são maiCs simples de configurar. Enquanto o Kubernetes oferece ferramentas integradas e uma vasta gama de opções para gerenciamento e monitoramento de clusters. No entanto, com uma configuração muito mais complexa.

## MongoDB vs PostgreSQL
Por último, vamos comparar duas tecnologias utilizadas para banco de dados, utilizando também 5 aspectos principais:

**Modelo de Dados:** O MongoDB é um banco de dados NoSQL orientado a documentos, ideal para dados semiestruturados ou não estruturados. Oferece flexibilidade no esquema de dados, permitindo que os desenvolvedores ajustem os dados de acordo com as necessidades da aplicação. E o PostgreSQL pe um banco de dados relacional (SQL) com forte suporte a estruturas de dados complexas e rigorosa integridade referencial. Ideal para aplicações que requerem transações ACID e dados altamente estruturados.

**Escalabilidade:** Enquanto o PostgreSQL escala verticalmente de forma eficaz, com suporte a replicação. Embora haja soluções para sharding, o PostgreSQL é mais frequentemente utilizado em cenários de escalabilidade vertical. O MongoDB escala horizontalmente de forma nativa, o que o torna ideal para grandes volumes de dados distribuídos. Suporta sharding, permitindo que os dados sejam divididos entre múltiplos servidores.

**Desempenho em Consultas Complexas:** Embora o MongoDB ofereça boas performances em consultas simples e operações de leitura/escrita, pode ser menos eficiente em consultas complexas devido à falta de otimizações SQL tradicionais. O PostgreSQL utiliza o Excel em consultas complexas e operações transacionais devido ao seu poderoso otimizador de consultas e suporte nativo a operações ACID. Normalmente, desempenha bem em cenários que exigem operações complexas entre tabelas.

**Maturidade e Comunidade:** O PostigreSQL é um dos bancos de dados mais antigos e maduros, com uma comunidade vasta e ativa, além de suporte sólido de documentação e ferramentas. Enquanto o MongoDB é relativamente mais novo, mas com uma comunidade crescente e uma ampla adoção em startups e empresas que precisam de flexibilidade de dados.

**Facilidade de COnfiguração e Administração:** O MongoDB é mias fácil de configurar, especialmente para desenvolvedores que necessitam de uma solução rápida e flexível. No entanto, a administração pode se tornar complexa em ambientes muito grandes. Já a configuração inicial do PostgreSQL pode ser mais complexa, especialmente devido à necessidade de planejamento de schema, mas oferece ferramentas robustas para administração, backup e recuperação.

# Atividade 3
![arquitetura da netflix](/Engenharia_de_Software/imagens/netflix-architecture.jpeg)

**Complexidade vs. Escalabilidade:** A arquitetura é altamente escalável, mas cada camada (microservices, armazenamento de dados, mensageria, etc.) adiciona complexidade que precisa ser gerida com cuidado.
**Agilidade vs. Custos de Manutenção:** A estrutura modular permite agilidade em mudanças e desenvolvimento, mas exige equipes especializadas para manter cada parte da arquitetura.
**Latência vs. Resiliência:** Garantir baixa latência em um sistema tão distribuído é desafiador, exigindo compensações em termos de resiliência e consistência de dados.

# Atividade 4
**Hospedagens de Cães**

## Diagrama
![arquitetura da netflix](/Engenharia_de_Software/imagens/HospedagemCaes.drawio.png)

## Classe: Cao
public class Cao {
    private String nome;
    private String raca;
    private int idade;

    public Cao(String nome, String raca, int idade) {
        this.nome = nome;
        this.raca = raca;
        this.idade = idade;
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public String getRaca() {
        return raca;
    }

    public void setRaca(String raca) {
        this.raca = raca;
    }

    public int getIdade() {
        return idade;
    }

    public void setIdade(int idade) {
        this.idade = idade;
    }

    public void exibirInformacoes() {
        System.out.println("Nome: " + nome + ", Raça: " + raca + ", Idade: " + idade);
    }
}

## Classe: Hospedagem
public class Hospedagem {
    private String nomeHospedagem;
    private int dias;
    private Cao cao;

    public Hospedagem(String nomeHospedagem, int dias, Cao cao) {
        this.nomeHospedagem = nomeHospedagem;
        this.dias = dias;
        this.cao = cao;
    }

    public void exibirDetalhesHospedagem() {
        System.out.println("Hospedagem: " + nomeHospedagem + ", Dias: " + dias);
        cao.exibirInformacoes();
    }
}

## Classe: Main
public class Main {
    public static void main(String[] args) {
        Cao cao = new Cao("Rex", "Golden Retriever", 5);
        Hospedagem hospedagem = new Hospedagem("Hotel Canino", 7, cao);
        hospedagem.exibirDetalhesHospedagem();
    }
}
