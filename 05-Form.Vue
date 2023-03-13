<template>
    <form action="">
        <div>
            <inputText/>
        </div>
        <div>
            <inputText/>
        </div>
        <div>
            <inputSubmit/>
        </div>


    </form>
</template>

<script>
 import inputText from './inputText'
 import inputSubmit from './Submit'

    export default {
        name: 'Form',
        components: {
            inputText,
            inputSubmit
        }
      
    }
</script>
