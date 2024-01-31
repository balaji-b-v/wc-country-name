<svelte:options tag="country-name" />
<script lang="ts">
  export let displaylocale;
  export let countrycode;

  let countryDisplayName
  $: if(displaylocale && countrycode){
    const regionNamesInDisplayLocale = new Intl.DisplayNames([displaylocale], { type: 'region' });
    countryDisplayName = regionNamesInDisplayLocale.of(countrycode)
  }
</script>
<div>
    {countryDisplayName}
</div>
