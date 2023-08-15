<script></script>

<template>
  <div id="terms">
    <p class="terms__section">
      <b>IMPORTANT NOTICE TO CLIENTS REGARDING CRYPTO CURRENCY PROHIBITION. </b> Please be advised
      that Tradeview Markets does not accept cryptocurrency for deposit into client accounts. All
      deposits to client accounts must be made in fiat currency, such as USD, JPY, EUR, GBP, CAD and
      MXN. Clients using third party payment providers are prohibited from depositing cryptocurrency
      into the Tradeview Markets account with the third party payment provider and then converting
      the crypto currency to fiat currency for further deposit into their account. Tradeview must be
      able to trace all deposits back to a regulated financial institution. Violations of this
      anti-money laundering compliance provision regarding the use of crypto currency as a source
      for deposit into your Tradeview Markets account will result in the immediate liquidation of
      all open positions in your account and the permanent closure of your account.
    </p>
    <p class="terms__section">
      There is a risk of loss in trading foreign currencies and it is not suitable for everyone. We
      are compensated for our services through the bid-ask spread. Tradeview is not responsible for
      any gains or losses on currency rates or exchanges during any transaction. Copyright© 2022.
      All rights reserved. <br /><br />
      The services and products offered by Tradeview Markets are not being offered within the United
      States (US) and not being oﬀered to US Persons, as defined under US law. The information on
      this website is not directed to residents of any country where FX and/or CFDs trading is
      restricted or prohibited by local laws or regulations. <br /><br />
      <b
        >Terms and Conditions | Privacy Policy | AML Policy | Withdrawal Policy | Refund Policy |
        Risk Disclosure | FAQ</b
      >
    </p>
    <div id="terms__grid" class="terms__section">
      <div>
        <h3 id="terms__grid-title">Tradeview Ltd.</h3>
        <br />
        <p id="terms_grid-description">
          Is licensed to carry on securities investment business and is regulated by the Cayman
          Islands Monetary Authority (CIMA) as a full securities broker-dealer. (License #585163)
          Tradeview conducts business pursuant to the Cayman Islands Securities Investment Business
          Law (SIBL) and its activities fall under the direct supervision of the Investments and
          Securities Division of CIMA
        </p>
        <br />
        <b>Website: <a id="terms_grid-url">www.tradeviewforex.com</a></b>
      </div>
      <div>
        <h3 id="terms__grid-title">TVM Global Ltd</h3>
        <br />
        <p id="terms_grid-description">
          Is licensed and regulated by the Labuan Financial Services Authority (FSA) as a Money
          Broker, registration number LL15870 licensed to facilitate transactions in foreign
          exchange pursuant to Labuan Financial Services and Securities Act 2010, the Labuan
          Companies Act 1990 and the Labuan Business Activity Tax Act 1990.
        </p>
        <br />
        <b>Website: <a id="terms_grid-url">www.tvmgloballtd.com</a></b>
      </div>
      <div>
        <h3 id="terms__grid-title">Tradeview Europe Ltd</h3>
        <br />
        <p id="terms_grid-description">
          Is licensed as a Category 2 Investment Service Company and is regulated by the Malta
          Financial Services Authority (MFSA). The Malta Financial Services Authority (MFSA) is the
          single regulator for financial services in Malta. MFSA is a fully autonomous public
          institution and reports to Parliament on an annual basis. The MFSA is a member of the
          European Banking Authority (EBA), the European Securities and Markets Authority (ESMA) and
          the International Organization of Securities Commissions (IOSCO) and is a signatory of the
          Multilateral Memorandum of Understanding with other European regulatory Institutions.
          Tradeview is authorized to provide financial services across multiple asset classes and is
          passported in the EU/EEA under MiFID II (EU Markets in Financial Instruments Directive).
        </p>
        <br />
        <b>Website: <a id="terms_grid-url">www.tradeview.eu</a></b>
      </div>
      <div>
        <h3 id="terms__grid-title">Tradeview Financial Markets S.A.C Global</h3>
        <br />
        <p id="terms_grid-description">
          s authorized to conduct business pursuant to and in compliance with the General Law of
          Companies (LGS) promulgated by the government of Peru. Tradeview Financial Markets S.A.C
          is registered with the National Superintendence of Public Registries (SUNARP), company
          number 13089531. Tradeview Financial Markets S.A.C provides financial services in selected
          OTC derivative markets in compliance with all applicable government regulations.
        </p>
        <br />
        <b>Website: <a id="terms_grid-url">www.tradeviewlatam.com</a></b>
      </div>
      <div>
        <h3 id="terms__grid-title">iLC Brokers Ltd</h3>
        <br />
        <p id="terms_grid-description">
          iLC Brokers Ltd. is authorized under the Mauritius Financial Service Commission with a
          Global Business License and Investment Dealer License #GB20025800 to provide financial
          services to professional and non-professional clients.
        </p>
        <br />
        <b>Website: <a id="terms_grid-url">www.ilcbrokers.com</a></b>
      </div>

      <div>
        <h3 id="terms__grid-title">TVCM Limited (Tradeview UK)</h3>
        <br />
        <p id="terms_grid-description">
          Is a limited company registered in England & Wales under Company Number 08648747 and is
          authorised and regulated by the Financial Conduct Authority FRN: 990586
        </p>
        <br />
        <b>Website: <a id="terms_grid-url"> www.tradeview.co.uk</a></b>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
b strong {
  color: var(--vt-c-white);
  font-weight: bold;
}
.terms {
  &__section {
    border-top: 1px solid gray;
    padding: 2em 0;
  }
}
#terms {
  display: flex;
  flex-direction: column;
  margin-top: 5em;
  color: var(--text-color-terms);

  &__grid {
    display: grid;
    gap: 10%;
    grid-template-columns: repeat(2, 1fr);
    &-title {
      text-decoration: underline;
      font-weight: bold;
    }
  }
}
</style>
