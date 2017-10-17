react-router是一个专为react提供的完整路由库。

history是一个js库，可以让您轻松地管理会话历史。


                             数据接入】

firebase是一个数据同步的云服务，帮助开发者开发具有【实时】特性的应用，让我们
实现真正的无后端编程。

reactfire：一个react的mixin库，封装了六个组件公共的方法，专门用于处理React和
Firebase集成的mixin方法，几行代码轻松获取数据。

npm install --save reactfire firebase
在代码中引入：
import ReactFireMixin from 'reactfire';
import Firebase from 'firebase';

可以用decorator的写法：
function testable(target) {
target.isTestable = true;
}
@Testable
class MyTestableClass {}
console.log(MyTestableClass.isTestable) //true

使用core-decorators提供的mixin来做重用模块的叠加，首先下载：
npm install --save core-decorators
然后在代码中引入就可以使用了
import { mixin } from 'core-decorators';
@mixin(ReactFireMixin)
class Profile extends Component {
...
}

配置.babelrc
{
"presets": ["es2015", "stage-0", "react"],
"plugins": ["transform-runtime", "transform-decorators-legacy"]
}

现在，我们可以在代码中使用reactfire这个mixin类库以及decorator语法。




                             请求数据

使用axios请求github API的数据

axios是一个能同时运行于浏览器端和nodejs的AJAX/HTTP方法/库




































