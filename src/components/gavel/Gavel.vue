<template>
  <div class="gavel">
    <q-card v-for="item in atuacao" :key="item.title" >
      <q-card-title>
        {{item.title}}
      </q-card-title>
      <q-card-separator />
      <q-card-main>
        <p>{{item.content}}</p>
      </q-card-main>
    </q-card>
  </div>
</template>

<script>
import { QCard, QCardTitle, QCardSeparator, QCardMain } from 'quasar'
export default {
  data: () => ({
    atuacao: [
      {
        title: 'Direito Civil',
        content: 'O principal corpo de normas objetivas do direito civil, no ordenamento jurídico brasileiro, é o Código Civil (Lei n. 10.406, de 10 de janeiro de 2002), que é dividido em duas partes: a parte geral e a parte especial.'
      },
      {
        title: 'Direito de Familiar',
        content: 'Direito de família é o ramo do direito que contém normas jurídicas relacionadas com a estrutura, organização e proteção da família. Ramo que trata das relações familiares e das obrigações e direitos decorrentes dessas relações, ou seja, é o ramo do Direito que regula e estabelece as normas de convivência familiar.' +
          'Dentro do Direito de Família, encontramos o Casamento, que é a união voluntária entre duas pessoas, formalizada nos termos da Lei, com o objetivo de manter uma plena comunhão de vida.' +
          'Em Portugal encontra-se regulado no livro quarto do Código Civil.' +
          'A matéria está regulada no Código Civil Brasileiro de 10 de Janeiro de 2002, nos artigos 1.511 a 1.783 (Livro IV - Do direito da família) e de 1.784 a 2.046 (Livro V - Do direito das sucessões).'
      },
      {
        title: 'Direito do Trabalho',
        content: 'Direito do trabalho é o conjunto de normas jurídicas que regem as relações entre empregados e empregadores, são os direitos resultantes da condição jurídica dos trabalhadores. Estas normas, no Brasil, estão regidas pela Consolidação das Leis do Trabalho (CLT), Constituição Federal de 1988 e várias leis esparsas (como a lei que define o trabalho do estagiário, dentre outras).'
      },
      {
        title: 'Revisional de Juros',
        content: 'Trata-se de demanda judicial através da qual o autor busca revisar determinadas cláusulas de um contrato. Neste artigo vamos abordar tão somente as ações revisionais de financiamento bancário. Nas ações revisionais de financiamentos bancários de regra são debatidos os seguintes temas abusividade da taxa de juros remuneratórios, forma de cobrança da comissão de permanência, tabela price, capitalização, TAC, vendas casadas.'
      },
      {
        title: 'Direito do Consumidor',
        content: 'O Direito do Consumidor é o ramo do direito que lida com as relações jurídicas entre fornecedores de bens e serviços e seus consumidores. Tem por objetivo assegurar que os consumidores obtenham acesso a informações quanto a origem e qualidade dos produtos e serviços; assegurar proteção contra fraudes no mercado de consumo; garantir transparência a segurança para os usuários dos bens e serviços e harmonizar as relações consumo por meio da intervenção jurisdicional. O direito do consumidor também assegura que o consumidor possa recorrer ao judiciário para a prevenção e reparação de danos patrimoniais decorrentes na falha no fornecimento de bens e prestação de serviços para o consumidor final.'
      }
    ]
  }),
  name: 'gavel',
  components: {
    QCard,
    QCardTitle,
    QCardSeparator,
    QCardMain
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus">
@import '~variables'
</style>
