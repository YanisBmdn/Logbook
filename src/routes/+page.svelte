<script>
    import { marked } from 'marked'
    import logbook from '../lib/md/logbook.md?raw'
</script>
<div class="content">
    {@html marked(logbook)}
</div>