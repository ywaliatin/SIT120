<template>
   <div id="filter">
      <h1> {{msg}} </h1>
<ul>
    <li v-for-key="item in filterList"> {{item.name}} - {{item.age}} </li>
</ul>
</div>
</template>

<script>
 export default {
     name:'hello',
    data (){
        return {
            msg: 'Testing Filter',
            
            filterList: [
                {
                    name:'test1',
                    age: 45,
                    suburb: 'bentleigh',
                    gender:'male'
                },
                {
                    name:'test2',
                    age: 40,
                    suburb: 'bentleigh',
                    gender:'female'
                },
                {
                    name:'test3',
                    age: 25,
                    suburb: 'sandringham',
                    gender:'male'
                },
                {
                    name:'test4',
                    age: 15,
                    suburb: 'sandringham',
                    gender:'female'
                }
            ]
        }
    }
 }

</script>



