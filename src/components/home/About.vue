<template>
  <v-container
    id="about"
    tag="section"
  >
    <v-layout row wrap>
      <v-flex align="center" flat v-for="card in cards" :key="`2${card}`" pa-4 pl-12 md3 xs6>
        <p flat class="bold">{{card.title}}</p>
        <p flat >{{card.subtitle}}</p>
        <p flat style="white-space: pre-line;">{{card.description}}</p>
      </v-flex>
    </v-layout>
    <p class="description">
        Linstock LLC is in the process of registering as an inter broker-dealer with FINRA and SIPC. Stocks are a high risk investment and have exhibited strong volatility. 
        <br/><br/><br/>

        Linstock is the brand name of the websites and digital platforms operated by Linstock LLC and its affiliated companies.
        <br/><br/><br/>

        Investors should consider the investment objectives, risks, and charges and expenses of an Exchange Traded Fund (“ETF”) carefully before investing. Before investing in any ETF, you should consider its investment objective, risks, charges and expenses. Contact us at help@linstock.us for a prospectus containing this information. Read it carefully. ETFs are subject to market fluctuation and the risks of their underlying investments. ETFs are subject to management fees and other expenses. ETF shares are bought and sold at market price, which may be higher or lower than their NAV, and are not individually redeemed from the fund. Investment returns will fluctuate and are subject to market volatility, so that an investor's shares, when redeemed or sold, may be worth more or less than their original cost. ETFs are subject to risks similar to those of stocks. Some specialized exchange-traded funds can be subject to additional market risks. Leveraged and inverse exchange-traded products are not designed for buy and hold investors or investors who do not intend to manage their investment on a daily basis.
        
        These products are for sophisticated investors who understand their risks (including the effect of daily compounding of leveraged investment results), and who intend to actively monitor and manage their investments on a daily basis.
        <br/><br/><br/>

        Be sure to consider your own financial situation, perform thorough research, and consult with a qualified tax professional before making any investment decisions concerning REITs. Investments in REITs and other real estate securities are subject to the same risks as direct investments in real estate. The real estate industry is particularly sensitive to economic downturns.
        <br/><br/><br/>
        ‍
        Where an investment is denominated in a currency other than the investor’s currency, changes in rates of exchange may have an adverse effect on the value, price of, or income derived from the investment.
        <br/><br/><br/>

        Securities products are: Not FDIC insured · Not bank guaranteed · May lose value
        <br/><br/><br/>

        Market data refreshed at least every 15 minutes unless otherwise indicated. Market data provided by IEX Group & Polygon
        <br/><br/><br/>
        ‍
        Trademarks and logos are the property of their respective owners and do not represent endorsements of any kind. Unless otherwise noted, Passfolio Securities, LLC and its affiliates are not partners, affiliates, or licensees of these companies.
        <br/><br/><br/>

        Linstock LLC
        <br/>
        V.1.0 06/30/2020
    </p>
  </v-container>
</template>

<script>
  export default {
    name: 'HomeAbout',
    data: () =>  ({
      cards: [
        {
          title: "COMPANY INFO",
          subtitle: "LINSTOCK LLC",
          description: "300 Spectrum Irvine, CA, 92618",
        },
        {
          title: "",
          subtitle: "LINSTOCK SECURITIES",
          description: "Gangnam-daero 364, \n Gangnam-gu, \n Seoul, S. Korea",
        },
        {
          title: "DOCUMENTS",
          subtitle: "Terms and Conditions",
          description: "Privacy Policy \n AML & KYC Rules",
        },
        {
          title: "CONNECT",
          subtitle: "Help",
          description: "Contact \n Facebook",
        },
      ],
    }),
  }
</script>

<style scoped>
.description {
  font-size: 12px;
}
.bold {
  font-weight: bold;
}
</style>
