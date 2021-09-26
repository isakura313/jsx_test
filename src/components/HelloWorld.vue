
<script>
export default {
  name: 'HelloWorld',
 data:()=>{
   return{
     info: "info",
      listOfItems: [
        {name:'list', key: 1},
        {name:'list 1', key: 2},
        {name:'list 2', key: 3}
      ]
   }
 },
  props: {
    msg: String
  },
  render(){
    return (
      <div>
      <h1> {this.info}</h1>
      <ul>
      <li for="item in this.listOfItems" key="index">{ item } </li>
      </ul>
      </div> 
    )
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
