react-router��һ��רΪreact�ṩ������·�ɿ⡣

history��һ��js�⣬�����������ɵع���Ự��ʷ��


                             ���ݽ��롿

firebase��һ������ͬ�����Ʒ��񣬰��������߿������С�ʵʱ�����Ե�Ӧ�ã�������
ʵ���������޺�˱�̡�

reactfire��һ��react��mixin�⣬��װ��������������ķ�����ר�����ڴ���React��
Firebase���ɵ�mixin���������д������ɻ�ȡ���ݡ�

npm install --save reactfire firebase
�ڴ��������룺
import ReactFireMixin from 'reactfire';
import Firebase from 'firebase';

������decorator��д����
function testable(target) {
target.isTestable = true;
}
@Testable
class MyTestableClass {}
console.log(MyTestableClass.isTestable) //true

ʹ��core-decorators�ṩ��mixin��������ģ��ĵ��ӣ��������أ�
npm install --save core-decorators
Ȼ���ڴ���������Ϳ���ʹ����
import { mixin } from 'core-decorators';
@mixin(ReactFireMixin)
class Profile extends Component {
...
}

����.babelrc
{
"presets": ["es2015", "stage-0", "react"],
"plugins": ["transform-runtime", "transform-decorators-legacy"]
}

���ڣ����ǿ����ڴ�����ʹ��reactfire���mixin����Լ�decorator�﷨��




                             ��������

ʹ��axios����github API������

axios��һ����ͬʱ������������˺�nodejs��AJAX/HTTP����/��




































