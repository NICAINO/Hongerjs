<script>
    import { metatags, url } from '@roxi/routify';
    metatags.title = 'My Routify app'
    metatags.description = 'Description coming soon...'
</script>

<body>
    <h1>Oops... Did you mean to go to the <a href={$url('./main')}>main page</a>?   </h1>
    
</body>