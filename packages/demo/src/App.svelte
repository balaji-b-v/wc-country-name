<script lang="ts">
  import CountryName from '../../lib/src/CountryName.wc.svelte';
</script>

<main>
  <h1>Display country names in desired locale!</h1><h2>Svelte components usage</h2>
  
  <!-- <p class="container"> -->
    <table>
      <thead>
        <tr>
          <td>Country Name in English</td>
          <td>Country Name in Arabic</td>
          <td>Country Name in German</td>
          <td>Country Name in Hindi</td>
          <td>Country Name in French</td>
        </tr>
      </thead>
      <tbody>
       
        <tr>
          <td><CountryName displaylocale="en" countrycode="DK"></CountryName></td>
          <td><CountryName displaylocale="ar" countrycode="DK"></CountryName></td>
          <td><CountryName displaylocale="de" countrycode="DK"></CountryName></td>
          <td><CountryName displaylocale="hi" countrycode="DK"></CountryName></td>
          <td><CountryName displaylocale="fr" countrycode="DK"></CountryName></td>
        </tr>
        <tr>
          <td><CountryName displaylocale="en" countrycode="US"></CountryName></td>
          <td><CountryName displaylocale="ar" countrycode="US"></CountryName></td>
          <td><CountryName displaylocale="de" countrycode="US"></CountryName></td>
          <td><CountryName displaylocale="hi" countrycode="US"></CountryName></td>
          <td><CountryName displaylocale="fr" countrycode="US"></CountryName></td>
        </tr>
        <tr>
          <td><CountryName displaylocale="en" countrycode="SG"></CountryName></td>
          <td><CountryName displaylocale="ar" countrycode="SG"></CountryName></td>
          <td><CountryName displaylocale="de" countrycode="SG"></CountryName></td>
          <td><CountryName displaylocale="hi" countrycode="SG"></CountryName></td>
          <td><CountryName displaylocale="fr" countrycode="SG"></CountryName></td>
        </tr>
        <tr>
          <td><CountryName displaylocale="en" countrycode="AE"></CountryName></td>
          <td><CountryName displaylocale="ar" countrycode="AE"></CountryName></td>
          <td><CountryName displaylocale="de" countrycode="AE"></CountryName></td>
          <td><CountryName displaylocale="hi" countrycode="AE"></CountryName></td>
          <td><CountryName displaylocale="fr" countrycode="AE"></CountryName></td>
        </tr>
        <tr>
          <td><CountryName displaylocale="en" countrycode="JP"></CountryName></td>
          <td><CountryName displaylocale="ar" countrycode="JP"></CountryName></td>
          <td><CountryName displaylocale="de" countrycode="JP"></CountryName></td>
          <td><CountryName displaylocale="hi" countrycode="JP"></CountryName></td>
          <td><CountryName displaylocale="fr" countrycode="JP"></CountryName></td>
        </tr>
      </tbody>   
    
    </table>
  <!-- </p> -->
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    font-size: 1.4em;
    line-height: 1.1;
    font-weight: 100;
  }
  table {
      width: 100%;
      border: 1px solid #100808;
  }
  thead{
    font-weight: bold;
  }
  td {
      border: 1px solid #eca0a0;
      padding: 10px;
  }
  h2{
        font-size: 1.1em;
        color: green;
      }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
    
  }
</style>