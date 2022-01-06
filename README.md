## Projeto de Estudo das 500 Mais da KISS FM
![](https://img.shields.io/badge/Python-3.8-blue.svg)
![](https://img.shields.io/badge/Pandas-blue.svg)

<img src="https://kissfm.com.br/wp-content/themes/KISSFM/img/kisslogo.png">

Kiss FM é uma emissora de rádio brasileira de São Paulo, capital do estado homônimo. Opera no dial FM, na frequência 92.5 MHz, e pertence à Rede Mundial de Comunicações, sendo a geradora da rede de rádios com emissoras em Santos e Rio de Janeiro. Seus estúdios estão localizados no Edifício The Central Park, no Espigão da Paulista, onde funcionam os demais veículos da Rede Mundial, onde também fica o transmissor.

Desde sua inauguração, em 2000, em Dezembro a rádio transmite o programa as 500 mais da KISS FM que uma lista das 500 músicas mais votas pelos ouvintes.

O programa não tem segredo – quem quiser, entra no site da emissora e vota em sua música predileta. As 500 músicas mais votadas são transmitidas no final do ano, de maneira interrupta. Por ser uma rádio, só vai votar quem ouve a rádio e, consequentemente, não podemos dizer que essa lista é um retrato do que o “público roqueiro” ou “público metaleiro” (principalmente esse segundo) ouve no geral. Com certeza, muita gente que votou são pessoas que ouvem rock não da mesma maneira que nós aqui do blog ouvimos, mas acho importante no começo de 2021 termos uma ideia de como o gênero e as bandas que carregam a bandeira são vistas (e ouvidas) pelo público brasileiro que se dispõe em participar dessa votação.

### Objetivo do estudo

- Levantar as bandas melhores rankeadas
- Levantas as músicas melhores rankeadas
- Agrupar os resultados por país de origem da banda
- Identificar quais músicas estiverem presentens em quais anos

### Configure seu ambiente

- crie um virtualenv e ative-o
- instale as dependências
- execute o jupyter lab

### Tratamento dos arquivos de 2000 a 2006

Os scripts estão no ```file_threat.ipynb```

Os arquivos entre 2000 e 2006 foram criados com o sufixo ```_orig``` e a lista das música é uma linha única.

Para usar no estudo, foi preciso criar um script para tratar esse dado e transformar esse única linha em múltiplas linhas

Exceto o arquivo 2000_orig.txt, os demais estão nesse formato
```
<ordem>. <Banda/Artista> - <Mùsica>
```

Arquivos de 2001 a 2005.

O que o algoritmo precisa fazer é localizar o vamor númerico da ordem antes do ponto, fazer um split até o próximo valor númerico e inserir uma quebra de linha ```\n```


Arquivo de 2006 não tem o ponto depois do número da ordem.

### Fonte

[Site Oficial das 500 da KISS FM](https://kissfm.com.br/as-500-mais-da-kiss/)

[Facebook](https://www.facebook.com/as500maisdakissfm/)

[Twitter](https://twitter.com/500maisdakissfm)

[Wikipedia - Kiss FM](https://pt.wikipedia.org/wiki/Kiss_FM)

[LeiteSPC](https://leitespc.blogspot.com/)

[MinutoHM](https://minutohm.com/2021/01/07/analise-das-500-mais-votadas-da-kiss-fm-em-2020/)