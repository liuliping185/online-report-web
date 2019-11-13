<template>
    <div id="warp">
        <form id="testForm" action="/online_report/declare/index" method="get">
            <ul>
                <li><lable>测试纳税人登记序号：</lable><input type="text" name="djxh" id="form_djxh" /></li>
                <li><label>凭证种类代码：</label><input type="text" name="pzzlDm" id="form_pzzlDm" /></li>
                <li><label>申报期：</label><input type="text" name="sbq" id="form_sbq" /></li>
            </ul>
        </form>
        <input type='button' value='按期申报' id='delcareBtn'>
        <hr/>
        <br/>
        <form id="amendForm" action="/online_report/amend/index" method="get">
            <ul>
                <li><lable>测试纳税人登记序号：</lable><input type="text" name="djxh" id="form_djxh_amend" /></li>
                <li><label>申报期：</label><input type="text" name="sbq" id="form_sbq_amend" /></li>
            </ul>
        </form>
        <input type='button' value='更正申报' id='amendBtn'><br/>
        <hr/>
        <br/>
        <form id="overdueForm" action="/online_report/overdue/index" method="get">
            <ul>
                <li><lable>测试纳税人登记序号：</lable><input type="text" name="djxh" id="form_djxh_overdue" /></li>
                <li><label>申报期：</label><input type="text" name="sbq" id="form_sbq" /></li>
            </ul>
        </form>
        <input type='button' value='逾期申报' id='overdueBtn'><br/>
        <hr/>
        <form id="cancellationForm" action="/online_report/overdue/index" method="get">
            <ul>
                <li><lable>测试纳税人登记序号：</lable><input type="text" name="djxh" id="form_djxh_cancellation" /></li>
                <li><label>申报期：</label><input type="text" name="sbq" id="form_sbq" /></li>
            </ul>
        </form>
        <input type='button' value='清册注销' id='cancellationBtn'><br/>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#warp {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin: 0 60px;
}
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 30px 0 5px 0;
}
li {
  margin: 10px 10px;
}
a {
  color: #42b983;
}
</style>
