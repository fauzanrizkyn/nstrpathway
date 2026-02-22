<script>
    import '../styles/global.css'
    import Navbar from '../components/navbar.svelte';
    import PageSection from '../components/pageSection.svelte';
    import PageSectionFlex from '../components/pageSectionFlex.svelte';
    
    
    import Home from '../components/pages/home.svelte';
    import Greenscreen from '../components/greenscreen.svelte';
    
    import About from '../components/pages/about.svelte';
    import Subjects from '../components/pages/subjects.svelte';
    import Books from '../components/pages/books.svelte';
    import Teams from '../components/pages/teams.svelte';
    import Roadmap from '../components/pages/roadmap.svelte';
    import Approach from '../components/pages/approach.svelte';

    import Footer from '../components/pages/footer.svelte';

</script>

<Greenscreen />
<Navbar></Navbar>
    <Home />
<PageSectionFlex>
    <About />
</PageSectionFlex>
<PageSectionFlex>
    <Subjects />
</PageSectionFlex>
<PageSectionFlex>
    <Books />
</PageSectionFlex>
<PageSectionFlex>
    <Teams />
</PageSectionFlex>
<PageSection>
    <Roadmap />
</PageSection>
<PageSectionFlex>
    <Approach />
</PageSectionFlex>
<Footer />

