<script context="module">
    // this is preloaded before the page is rendered, it is primarly used for loading data
    export async function preload(page){
        return { state : page.params['state']};
    }
</script>
<script>
    import CovidChart from '../components/CovidChart.svelte';
    import CovidStat from '../components/CovidStat.svelte';
    import TableContainer from '../components/TableContainer.svelte'
    export let state;
</script>
    


<h1>{state}</h1>
<CovidStat />
<CovidChart />