<div id="value"></div>

<script>
    async function getVistor(params) {
        await fetch('https://api.countapi.xyz/hit/gilangzyehan.com/github', {
            method: 'GET'
        }).then((res) => res.json())
            .then((res) => {
                console.log(res)
                value.innerText = res.value
            })
    }
    getVistor()
</script>
