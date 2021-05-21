<template>
  <v-app>
    <div class="wrapper">
      <div class="section1" id="About">
        <v-container>
          <v-row>
            <v-img
              width="1000"
              height="711"
              src="https://professorwerner.org/wp-content/uploads/2016/11/richard_werner_speech_4_s.jpg"
            >
            </v-img>
          </v-row>
        </v-container>
      </div>
      <div class="section2">
        <v-container>
          <h2>Biography</h2>
          <div class="bottom-border"></div>
          <p class="paragraph-text">
            Professor Richard A. Werner, born in Germany in 1967, holds a First
            Class Honours B.Sc. in Economics from the London School of Economics
            and a doctorate in Economics from the University of Oxford. He has
            also studied at the University of Tokyo. 
          </p>
            <p class="paragraph-text">
              Richard is a Member of
            Linacre College, Oxford, and is a university professor in banking
            and finance. He is also a founding chair of Local First, a community
            interest company establishing not-for-profit community banks in the
            UK (including the Hampshire Community Bank). His recommended charity
            is the Association for Research on Banking and the Economy
            (www.arbe.org.uk). You can follow him on Twitter @scientificecon .
            </p>
            <p class="paragraph-text">
            Until February 2019, Richard was for many years a member of the ECB
            Shadow Council. In 2008 he founded, and has been director of the
            Centre for Banking, Finance and Sustainable Development – the first
            research centre to focus on the link between the financial sector
            and sustainability issues. Between 2009 and 2012 for five semesters
            he was a full-time professor of monetary, macro and development
            economics (W3) at Goethe-University Frankfurt. Until July 2018 he
            was Professor of International Banking at the University of
            Southampton (having joined in April 2004). From 1997 to 2004 he was
            assistant professor in economics and finance at Sophia University,
            Tokyo (one of Japan’s top 3 private universities). 
            </p>
            <p class="paragraph-text">
            He has also
            taught development finance and sustainability at Moscow State
            University, as well as a range of economics, banking and finance
            courses at a number of other universities. His work experience
            includes over four years as highly-rated chief economist at Jardine
            Fleming Securities (Asia) Ltd., a stint as Senior Managing Director
            at Bear Stearns Asset Management Ltd., many years managing global
            macro funds, several years as senior consultant to the Asian
            Development Bank and periods as visiting scholar and visiting
            researcher at the Japanese Ministry of Finance and the Bank of
            Japan, respectively. He was also the first Shimomura Fellow at the
            Development Bank of Japan. In 1992, while European Commission Fellow
            at Oxford University’s Institute for Economics and Statistics,
            Richard proposed the disaggregation of credit and its impact on
            asset markets and growth with his ‘Quantity Theory of Credit’ (see
            here). 
            </p>
            <p class="paragraph-text">
            In 1995, he advanced the concept of ‘quantitative easing’ in
            Japan (defined as an expansion in credit creation, published in the
            leading daily newspaper, the Nikkei, on 2 September 1995). His book
            ‘Princes of the Yen’ was a No. 1 bestseller in Japan, beating Harry
            Potter for six weeks. In its English edition of 2003, he warned of
            the coming creation of credit bubbles and banking crises in the
            eurozone. So did his 2005 book ‘New Paradigm in Macroeconomics’
            (Palgrave Macmillan). In 2014, Richard published the first empirical
            proof of the fact that banks create money when they grant loans. The
            World Economic Forum, Davos, selected him as “Global Leader for
            Tomorrow” in 2003.
          </p>
        </v-container>
      </div>
      <v-container>
        <v-row>
          <v-col cols="12" lg="6">
            <div class="section4-content">
              <h2>Education & Training</h2>
              <div class="bottom-border"></div>
              <h3>
                To ensure clients full satisfaction and positive feedback as we
                deliver services that is beyond expectation and create a long
                term loyal relationship by consistently providing outstanding
                services.
              </h3>
            </div>
          </v-col>
         <v-col cols="12" lg="6">
            <div class="section4-content">
              <h2>Education & Training</h2>
              <div class="bottom-border"></div>
              <h3>
                To ensure clients full satisfaction and positive feedback as we
                deliver services that is beyond expectation and create a long
                term loyal relationship by consistently providing outstanding
                services.
              </h3>
            </div>
          </v-col>
        </v-row>
      </v-container>
      <v-container class="section5">
        <h2>GALLERY</h2>
        <v-row>
          <v-col v-for="n in 4" :key="n" class="d-flex child-flex" cols="3">
            <v-img
              :src="require(`../assets/${n}.jpg`)"
              aspect-ratio="1"
              class="grey lighten-2"
            >
              <template v-slot:placeholder>
                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-progress-circular
                    indeterminate
                    color="grey lighten-5"
                  ></v-progress-circular>
                </v-row>
              </template>
            </v-img>
          </v-col>
          <v-col cols="12" class="text-center">
            <v-btn class="red lighten-1">
              <router-link to="/Gallery" class="custom-btn">
                View More...
              </router-link>
            </v-btn>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </v-app>
</template>
<script>
export default {};
</script>
<style scoped>
.wrapper {
  padding: 70px 10%;
}
.paragraph-text{
  padding-top:30px;
  line-height: 1.428571429;
  color:#333333;
  
}
p{
      margin: 0 0 10px;
}
.section1-content h2,
.section2 h2,
.section4-content h2 {
  color: #293e40;
  font-size: 35px;
  font-weight: 550;
  padding-top: 30px;
  padding-bottom: 10px;
}
.section1-content h3,
.section2 h3,
.section4-content h3 {
  color: #293e40;
  font-size: 20px;
  font-weight: 300;
  padding-top: 10px;
  padding-bottom: 30px;
  text-align: center;
}
.section2 {
  padding-top: 60px;
  text-align: left;
}
.bottom-border {
  position: relative;
  margin: 0 auto;
  width: 100%;
  height: 3px;
  background: #f82200;
  border-left: 23px solid #fcafa3;
  opacity: 0.9;
}
.section2 a {
  text-decoration: none;
  color: #293d40;
}
.custom-btn {
  text-align: center;
  padding: 10px 0;
  font-size: 16px;
  text-decoration: none;
  color: #ffffff;
}
/* .custom-btn:hover {
} */
.section4-content {
  padding-top: 50px;
  padding-bottom: 70px;
  padding-right: 20px;
  padding-left: 20px;
  text-align: center;
}
.section5 h2 {
  color: #293e40;
  font-size: 45px;
  font-weight: 550;
  padding-top: 30px;
  padding-bottom: 10px;
  text-align: center;
}
.section5 {
  margin-bottom: 200px;
}
@media only screen and (max-width: 600px) {
  .section4-content-img {
    width: 90%;
  }
  .section1-content {
    padding-top: 6px;
    padding-bottom: 2px;
    padding-right: 2px;
    padding-left: 2px;
  }
  .section4-content h3 {
    padding-bottom: 3px;
  }
}
</style>