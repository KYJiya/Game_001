<script>
    import fastapi from "../lib/api"

    let message = [];
    
    function hello() {
        fastapi('get', '/hello', {}, (json) => {
            message = json
        })
    }

    hello()
</script>


<div class="container my-3">
    {message.message}
</div>