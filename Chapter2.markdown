#�ĤG�� Angular���ε{����R

�����嫬���禡�w, �A�ݭn�D��A���w���\��, �bAngular���Ҧ����F�賣�Q�]�p���@�ӥΩ��@���M��. �b�������ڭ̱N�[�\Angular���Ҧ����򥻺c�ض�, �o�˧A�N�i�H�z�Ѧp��N���̲զX�b�@�_. �o�Ƕ����N�b�᭱�����`������ԲӪ��Q��.

##�ҥ�Angular

�������ε{�������������ƨӱҥ�Angular:

1. �[��`angular.js`�w
2. �ϥ�`ng-app`���O�ӧi�DAngular�����Ӻ޲z������DOM

###�[���}��

�[���w��²��, �P�[����L����JavaScript�w��`�P�˪��W�h. �A�i�H�qGoogle�����e���o����(CDN)�����J�}��, �N���o��:
```html
    <script src="http://ajax.google.com/ajax/libs/angularjs/1.0.4/angular.min.js"></script>
```
���˨ϥ�Google��CDN. Google�����A���ܧ�, �åB�o�Ӹ}���O�����ε{���֨���. �o�N����, �p�G�A���Τᦳ�h�����ε{���ϥ�Angular, ����L�N�u�ݭn�U���}���@��. ���~, �p�G�Τ�X�ݹL��L�ϥ�Google CDN�s��Angular�����I, ����L�b�X�ݧA�����I�ɴN���ݭn�A���U���Ӹ}��.

�p�G�A����w���a�D��(�Ϊ̨�L���覡), �A�]�i�H�o�˰�. �u�ݭn�b`src`�����w���T���a�}.

###�ϥ�ng-app�n��Angular���ɭ�

> ���OBoundaries, �N��O�n�����ε{�����@�ΰ�, �YAngular���ε{�����@�νd��.

`ng-app`���O�Ω����A�i�DAngular�A���楦�޲z������������. �p�G�A�b�إߤ@�ӧ�����Angular���ε{��, ����A���Ӧb`<html>`���Ҥ��]�t`ng-app`����, �N���o��:
```html
    <html ng-app>
    �K
    </html>
```
�o�|�i��Angular�n�޲z���������Ҧ�DOM����. 

�p�G�A���@�Ӳ{�������ε{��, �n�D�ϥΨ�L���޳N�Ӻ޲zDOM, �ҦpJava�Ϊ�Rails, �A�i�H�g�ѱN����m�b�������@�Ǥ����Ҧp`<div>`���ӧi�DAngular�u�ݭn�޲z�������@�����Y�i.
```html
    <html>
    �K
        <div ng-app>
        �K
        </div>
    �K
    </html>
```
###�ҫ�/����/���

�b�Ĥ@����, �ڭ̴���Angular����ҫ�/����/��������ε{���]�p����. ���M�b�]�p�A��Angular���ε{���ɦ��ܤj���F����, ���O�`�O�O���@�f������:

+ �ҫ��]�t�N��A�����ε{����e���A�����
+ ������ܸ��
+ ����޲z�A���ҫ��M���Ϥ��������Y

�A�ݭn�ϥιﹳ�ݩʪ��覡�إ߼ҫ�, �Ϊ̥u�]�t��l���������. �o�̨èS���S�w���ҫ��ܼ�. �p�G�A�Ʊ浹�Τ���ܤ@�Ǥ�r, �A�i�H�ϥΤ@�Ӧr�Ŧ�, �N���o��:
```js
    var someText = 'You have started your journey';
```
�A�i�H�g�ѽs�g�@�Ӽ˪O�@��HTML����, �ñq�ҫ����X�ָ�ƪ��覡�ӫإߵ���. ���p�ڭ̤w�g�ݹL��, �A�i�H�bDOM�����J�@�Ӧ����, �M��A���o�˳]�w������r:
```html
    <p>{{someText}}</p>
```
�ڭ̩I�s�o�����j�A���y�k�Ӵ��J��, ���N���J�s�����e��@�Ӳ{�����Ҫ���.

����N�O�A�s�g�Ω�i�DAngular���ǹﹳ�M��l�Ⱥc���A���ҫ�����, �g�ѱN�o�ǹﹳ�Ϊ̭�l�Ȥ��t��`$scope`�ﹳ�ǻ��챱���.
```js
    function TextController($scope){
        $scope.someText = someText;
    }
```
��L�̩�b�@�_, �ڭ̱o��p�U�N�X:
```html
    <html ng-app>
    <body ng-controller="TextController">
        <p>{{someText}}</p>
        
        <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.0.1/angular.min.js"></script>
        
        <script>
            function TextController($scope){
                $scope.someText = 'You have started your journey';
            }
        </script>
    </body>
    </html>
```
�N�����J���s������, �A�N�|�ݨ�

> 'You have started you journey'

���M�o�ӭ�l���檺�ҫ��u�@�b²�檺���p�U, �M�Ӥj�h�ƪ����ε{���A���Ʊ�إߤ@�Ӽҫ��ﹳ�ӥ]�q�A�����. �ڭ̱N�إߤ@�ӰT���ҫ��ﹳ, �åΥ��Ӧs�x�ڭ̪�`someText`. �]�����O�o�˪�:
```js
    var someText = 'You have started your journey';
```
�A���ӳo�˽s�g:
```js
    var messages = {};
    messages.someText = 'You have started your journey';
    function TextController($scope){
        $scope.messages = messages;
    }
```
�M��b�A���˪O���o�˨ϥ�:
```html
    <p>{{messages.someText}}</p>
```
���p�ڭ̫᭱�|�ݨ�, ��ڭ̰Q��`$scope`�ﹳ��, ���o�˫إߤ@�Ӽҫ��ﹳ�N���Q�󨾤�q`$scope`��H���쫬���~�Ӫ��N�~�欰.

�ڭ̥��b�Q�ת��o�Ǥ�k�q�����ݨӯ�����U�A, �b�W�����Ҥl��, �ڭ̦b����@�ΰ줤�إߤF`TextController`. ���M�o�O�@�ӫܦn���Ҥl, ���O���T�w�q�@�ӱ�������k���ӬO�N���@���Ҳժ��@����, �����A�����ε{���������ѤF�@�өR�W�Ŷ�. ��s���᪺�N�X�ݰ_�����ӬO�U���o��.
```html
    <html = ng-app="myApp">
    <body ng-controller="TextController">
        <p>{{someText.message}}</p>
        
        <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.0.1/angular.min.js"></script>
        
        <script>
            var myAppModule = angular.module('myApp',[]);
            
            myAppModule.controller('TextController', function($scope){
                var someText = {};
                someText.message = 'You have started your journey';
                $scope.someText = someText;
            });
        </script>
    </body>
    </html>
```
�b�o�Ӫ�����, �ڭ��n���Ҳդ�`ng-app`�������W�٬�`myApp`. �M��ڭ̩I�sAngular�ﹳ�إߤF�@�ӦW��myApp���Ҳ�, �M��I�s�Ҳժ�`controller`��k�ñN�ڭ̪������ƶǻ�����.

�@�|��ڭ̴N�|���D������, �H�Φp����o�Ҧ����Ҳ�. ���O�{�b, �u�ݭn�O��N�Ҧ����T�����O�s�b���쪺�R�W�Ŷ����O�@��n��, �åB�o�]�O�ڭ̨ϥμҲժ�����.

##�˪O�M���ô��

�bAngular���ε{�����˪O�u�OHTML���, �N���ڭ̱q�q�A�Ⱥݸ��J�Ϊ̩w�q�b`<script>`���Ҥ��������L�R�A�귽�@��. �b�A���˪O���w�q�Τ�ɭ�, �i�H�ϥμзǪ�HTML�[Angular���O�өw�q�A�һݭn��UI�ե�.

�@���i�J�s������, Angular�N�|�i�J��A��������ε{�����g�ѦX�ּ˪O�M��ƪ��覡�ӸѪR�o�Ǽ˪O. �b�Ĥ@�����ڭ̤w�g�b�ʪ������Τ��ݹL�F��ܤ@�Ӷ��ئC���Ҥl.
```html
    <div ng-repeat="item in items">
        <span>{{item.title}}</span>
        ...
    </div>
```
�o��, ���u�O�~�h`<div>`���@�Ӱƥ�, �̭��Ҧ����@��, ���@�@����`items`�Ʋդ����C�Ӥ���.

����o�Ǹ�Ʊq���̨�? �b�ڭ̪��ʪ����Ҥl��, �b�ڭ̪��N�X���ڭ̥u�N���w�q���@�ӼƲ�. ���A�}�l�إߤ@��UI�çƱ���ե��O�p��u�@��, �o�O�D�`�X�A��. �M�Ӥj�h�ƪ����ε{��, �N�ϥΤ@�Ǧ��A���W�����[�ʸ��. �b�s�������A�����ε{���s���A�����A��, �Τ�b�����W�ШD�L�̩һݭn���@��, �M��Angular�N��[�ШD�����]�P�A���˪O�X��.

�򥻪��B�@�y�{�ݰ_�ӹ��o��:

1. �Τ�ШD�A�����ε{�����Ĥ@�ӭ���
2. �Τ��s�����o�X�@��HTTP�ШD�s����A�����A��, �M��[���]�t�˪O��*index.html*����
3. Angular���J�쭶����, ���쭶�������[��, �M��d�ߩw�q�b�˪O�d�򤺪�`ng-app`
4. Angular�M���˪O�ìd�߫��O�M�j�w. �o�N�ɭP���U�ƥ��ť���MDOM�ާ@, �H�αq���A���W���o��l���. �o���u�@���̲׵��G�O�i�����ε{���ñN�˪O�@��DOM�ഫ������.
5. �s����A�����A���[���A�ݭn�i�ܵ��Τ�һݪ����[���.

��1�B�ܲ�3�B�O�C��Angular���ε{�����з�. ��4�B�M��5�B��A�ӻ��O�i�諸. �o�ǨB�J�i�H�P�B�Ϊ̫D�P�B�o��. �X��ʯ઺�Ҽ{, �A���ε{���һݪ���Ʀb�Ĥ@�ӵ��Ϥ�[����]��ܵ��Τ�, �i�H��֨��קK���ƪ��ШDHTML�˪O.

�g�Ѩϥ�Angular��´�A�����ε{��, �A�i�H�b�A�����ε{���������˪O�M���. �o�˰������G�O�o�Ǽ˪O�O�i�H�֨���. �b�Ĥ@�����J����, ���W�s�������N�u�ݭn�ШD�s����ƤF. ���pJavaScript, �Ϥ�, CSS�H�Ψ�L�귽, �֨��o�Ǽ˪O�i�H���A�����ε{�����ѧ�n���ʯ�.

###��ܤ�r

�A�i�H�ϥ�`ng-bind`���O�b�AUI������a����ܩM��s��r. ������ص������Φ�. �@�جO�ڭ̨��L���j�A���Φ�:
```html
    <p>{{greeting}}</p>
```
�M��N�O�@�ӳQ�٬�`ng-bind`������ݩʪ����O:
```html
    <p ng-bind="greeting"><p>
```
�o��̪���X�O������. �p�G�ҫ������ܼ�`greeting`�]�w��"Hi, there", Angular�N���ͳo�˪�HTML:
```html
    <p>Hi, there</p>
```
�s�����N���"Hi, There".

���򬰤���A�|�ϥΤW�����t�~�@�اΦ�? �ڭ̫إߪ����A�����J�Ȫ��y�kŪ�_�ӧ�[�۵M�åB�u�ݭn��֪���J. ���M��اΦ����ͬۦP����X, ���ϥΤj�A���y�k, �[���A���ε{�����Ĥ@�ӭ���`index.html`��, �bAngular������A��������Ƥ��e, �Τ�i��|�ݨ�@�ӥ���V���˪O. �H�᪺���ϱN���|�g���o�@�I.

��]�O�s�����[��HTML����, ��V��, ���쨺��Angular�~�i��ǳƸѪR����.

�n�����O�A���M�i�H�b�j�h�Ƽ˪O���ϥ�`{{ }}`. �M��, �b�A��`index.html`�������j�w���, ���Өϥ�`ng-bind`. �o��, �����ƥ[�����A���Τ�N����]�ݤ���.

###����J

�bAngular���B�z��椸���O��²�檺. ���p�ڭ̨��L���X�ӨҤl, �A�i�H�ϥ�`ng-model`�ݩʸj�w��A���ҫ��ݩʤ����W. �o�A�Ω�Ҧ��зǪ���椸��, �Ҧp��r��J��, �����A, �_��ص���.  �ڭ̥i�H���o�˸j�w�@�Ӵ_��ب�@���ݩ�:
```html
    <form controller="SomeController">
        <input type="checkbox" ng-model="youCheckedIt">
    </form>
```
�o�N����:

1. ��Τ��ܴ_���, `SomeController`��`$scope`���@�ӦW��`youCheckedIt`���ݩʱN�ܦ�true. ������ܮɨ�`youCheckedIt`�ܦ�false.
2. �p�G�A�b`SomeController`���]�w`$scope.youCheckedIt`��true, �o�Ӵ_��ئbUI���|�Q�۰ʿ��. �]�w����false�h�������.

�{�b�ڷQ�����O�ڭ̯u���Q�n���O, ��Τᰵ�F�@�Ǥ���Ʊ��ɧ@�X�^��. ����r��J�ؤ���, �A�ϥ�`ng-change`�ݩʨӫ��w�@�ӱ����k, ����L�פ���ɭԥΤ���ܿ�J�ت��Ȯ�, �o�ӱ����k�����ӳQ�I�s. ���ڭ̰��@��²�檺�p�⾹�����U�Τ�ۤv�z�ѥL�̻ݭn�h�ֿ��~��o��Y�ǪF��:
```html
    <form ng-controller="StartUpController">
        Starting: <input ng-change="computeNeeded()" ng-model="funding.startingEstimate">
        Recommendation: {{funding.needed}}
    </form>
```
���ڭ̳o��²�檺�Ҥl, ���ڭ̥u�]�w��X�Τ�w��Q������. �ڭ��ٱN�]�w�@���q�{��0���ȨӶ}�l:
```js
    function StartUpController($scope){
    
        $scope.funding = { startingEstimate: 0 };
        
        $scope.computeNeeded = function(){
            $scope.needed = $scope.startingEstimate * 10;
        };
        
    }
```
�M��, �e�����N�X�����@�Ӽ�b���������D. ���D�O��Ω�b��r��J�ؤ���J�ɧڭ̥u�O���s�p��F�һݪ����B. �p�G�o�ӿ�J�إu�b�Τ�b�o�ӯS�w����J�ؤ���J�ɧ�s, �o�u�@�o�ܦn. ���O�p�G��L����J�ؤ]�b�ҫ����j�w�F�o���ݩʷ|��˩O? �p�G���q���A�����o��ƨӧ�s�S�|���?

�L�׳o�Ӧr�q�p���s, �ڭ̭n�ϥΤ@�ӦW��`$watch()`��`$scope`���[$scope��H����k]. �ڭ̱N�b�������᭱�ԲӰQ��`watch`��k. �򥻪��Ϊk�O, �i�H�I�s`$watch()`�õ��L�ǻ��@�Ӻʱ���F���M�@�ӥΩ�^����F���ܤƪ��^�I���.

�b�o�ر��p�U, �ڭ̧Ʊ�ʱ�`funding.startEstimate`�H�ΨC�����ܮɩI�s`computeNeeded()`. �M��ڭ̨ϥγo�Ӥ�k���g�F`StartUpController`.
```js
    function StartUpController($scope){
    
        $scope.funding = { startingEstimate: 0 };
        
        $scope.computeNeeded = function(){
            $scope.needed = $scope.startingEstimate * 10;
        };
        
        $scope.$watch('funding.startingEstimate', computeNeeded);
        
    }
```
�`�N�޸������ʱ���F��. �O��, ���O�@�Ӧr�Ŧ�. �o�Ӧr�Ŧ�O�����Y�ǪF����檺Angular��F��. ��F���i�H�i��²�檺�B��M�X��`$scope`��H���ݩ�. �b�������᭱�ڭ̷|�[�\��h�����F�����T��.

�A�]�i�H�ʱ��@�Ө�ƪ�^��, ���O���ä��|�ʱ�`funding.startingEstimate`, �]������Ȭ�0, �åB0[��l��]���A�|����.

�M��, �ѩ�C��ڭ̪�`funding.statingEstimates`���ܮ�`funding.needed`���|�۰ʧ�s, �ڭ̥i�H���o�˽s�g�@�ӧ�²�檺�˪O.
```html
    <form cn-controller="StartUpController">
        Starting: <input ng-model="funding.startEstimate">
        Recommendation: {{funding.needed}}
    </form>
```
�b�Y�Ǳ��p�U, �A�ä��Ʊ�C�@�ӧ��ܳ��o�ͦ^��, �ۤ�, �A�Ʊ浥��Τ�ӧi�D�A���ǳƦn�F. �Ҧp�i�৹���ʶR�Ϊ̵o�e�@�Ӳ�ѰO��.

�p�G�A����椤���@�տ�J��, ����A�i�H�b�o�Ӫ��W�ϥ�`ng-submit`���O�������w�@�Ӵ�����ɪ��^�I���. �ڭ̥i�H���Τ�g���I���@�ӫ��s�ШD���U�L�̱Ұ����Ϊ��覡���X�R�W�����Ҥl:
```html
    <form ng-submit="requestFunding()" ng-controller="StartUpController">
        Starting: <input ng-change="computeNeeded()" ng-model="startingEstimate">
        Recommendation: {{needed}}
        <button>Fun my startup</button>
    </form>
```
```js
    function StartUpController($scope){
        $scope.conputedNeeded = function(){
            $scope.needed = $scope.startingEstimate * 10;  
        };
        
        $scope.requestFunding = function(){
            window.alert("Sorry, please get more customers first.");
        };
    }
```
����մ���o�Ӫ���, `ng-submit`���O�]�|�۰ʪ����s�����B�z���q�{��`POST`�欰.

> ��妹�B�����~, ��洣�檺�q�{�欰�O`GET`.

�b�ݭn�B�z��L�ƥ󪺱��p�U, �N����A�Q�n���ѥ椬�Ӥ��O������@��, Angular���ѤF�������s������ͨƥ��ݩʪ��ƥ�B�z���O. ���`onclick`, �A���Өϥ�`ng-click`. ���`ondblclick`�A���Өϥ�`ng-dblclick`����.

�ڭ̥i�H���ճ̫�@���X�R�ڭ̪��p�⾹�Ұ�����, �ϥΤ@�ӭ��m���s�Ω�N��J�ت��ȭ��m��0.
```html
    <form ng-submit="requestFunding()" ng-controller="StartUpController">
        Starting: <input ng-change="computeNeeded()" ng-model="StartingEstimate">
        Recommendation: {{need}}
        <button>Fund my startup!</button>
        <button ng-click="reset()">Reset</button>
    </form>
    
    function StartUpController($scope){
    
        $scope.computeNeeded = function(){
            $scope.needed = $scope.startEstimate * 10;
        };
        
        $scope.requestFunding = function(){
            window.alert("Sorry, please get more customers first");
        };
        
        $scope.reset = function(){
            $scope.startEstimate = 0;
        }
    
    }
```
###�����JavaScript���@�Ǹ�

�b�AJavaScript�}�o�ͲP���Y�Ǯɨ�, ���H�i��|�i�D�A, �A���ӽs�g"�����JavaScript", �b�A��HTML���ϥ�`click`, `mousedown`�H�Ψ�L���������p�ƥ�B�z�{�ǬO���n��. ����L�O���T.

�����JavaScript��Q�w�g���ܦh����, ���O��s�X���檺��z�j�P�p�U:

1. ���O�C�ӤH���s���������JavaScript. ���C�ӤH������ݨ�A�Ҧ������e�M�ϥΧA�����ε{��, �Ӥ��ݭn�b�s����������N�X.

2. ���ǤH�ϥΪ��s�����u�@�覡���P. ���٤H���ϥΪ��ù��\Ū���M�@�Ǥ���Τ�ä���ϥκ�����JavaScript.

3. JavaScript�b���P�����x�u�@����@��. IE�s�����q�`�O�o��׭�. �A�ݭn�ھ��s���������P�ӨϥΤ��P���ƥ�B�z�N�X.

4. �o�Ǩƥ�B�z�{�ǤޥΥ���R�W�Ŷ��������. ��A���վ�X��L�w�����P�W��Ʈ�, ���|���A�Y�k.

5. �o�Ǩƥ�B�z�{�ǦX�֤F���c�M�欰. �o�ϧA���N�X��[���H���@, �X�R�M�z��.

�`��Ӭ�, ��A���ӳo�ح���s�gJavaScript�N�X, �@�����ܦn. �M�Ӧ��@��ƨä��O�n��, ���N�O�N�X�������שM�iŪ��. �ä��O�������n���ƥ�B�z�{�Ǥ��_�@��, �A�q�`���o�Ǥ������t�FID, ��o�o�Ǥ������ޥ�, �õ����]�w�F�ƥ�B�z���^�I���. �A�i�H�o���@�ӵ��c�u�Ω�M�����гy���̤��������p, ���j�h�����ε{��������]�w�b�U�B���ƥ�B�z���.

�bAngular��, �ڭ̨M�w���s�f���o�Ӱ��D.

�b�o�Ƿ����ϥͥH�ӥ@�ɴN�w�g���ܤF. ��1�I, �o�����쪺�s��w�g���A���F. �p�G�A�B�檺�s���������JavaScript, ����A���ӥh�ϥ�20�@��90�~�N�إߪ�����. �ܩ��2�I, �{�N���ù��\Ū���w�g��W�ӤF. �H��RAIA�y�q���Ҫ����T�ϥ�,  �A�i�H�гy���X�ݪ��IUI����. �{�b����W�B��JavaScript�P�]��x������۴��ýפF.

�]���{�b�����D�O: ���s��_���p�޳N�ӸѨM�ڭ̲�3�I�M��4�I���iŪ�ʩM²��ʪ����D��? 

���p�e���Ҵ��쪺, ���j�h�ƪ����p�ƥ�B�z�{��, Angular�����@�ӵ����Φ���`ng-eventhandler="expression"`�Ӵ��N`click`, `mousedown`, `change`���ƥ�B�z�{��. ��Τ��I���@�Ӥ�����, �p�G�A�Ʊ�o��@�Ӧ^��, �A�u�ݭn²�檺�ϥ�`ng-click`�o�˪����O:
```html
    <div ng-click="doSomething()">�K</div>
```
�A���j���̥i��|��"��, �o�˨ä��n"? �n�����O�A�i�H���P�U��. �o�ǫ��O���P�󥦭̨ƥ�B�z�{�Ǫ��e��(�зǨƥ�B�z�{�Ǫ���l�Φ�):

+ �b�C���s���������欰�@�P. Angular�|���A�B�z�n�t��.

+ ���|�b����R�W�Ŷ��ާ@. �A�ҫ��w����F���ȶȯ���X�ݤ�������@�ΰ줺����ƩM���.

�̫�@�Iť�_�ӥi�঳�I����, �]�����ڭ̨Ӭݤ@�ӨҤl. �b�@�Ө嫬�����ε{����, �A�|�إߤ@�Ӿɯ���M�@���H�ۧA�q�ɯ����ܤ��P�����ܤƪ����e��. �ڭ̥i�H�o�˽s�g�����ج[:
```html
    <div class="navbar" ng-controller="NavController">
    �K
        <li class="menu-item" ng-click="doSomething()">Something</li>
    �K
    </div>
    
    <div class="contentArea" ng-controller="ContentAreaController">
    �K
        <div ng-click="doSomething()">�K</div>
    �K
    <div>
```
�o�̷�Τ��I��navbar����`<li>`�Mconent�Ϥ���`<div>`�ɳ��|�I�s�@�Ӻ٬�`doSomething()`�����. �@���}�o�H��, �A�]�w�Ө�ƩI�s�A����������N�X�ޥ�. ���̥i��O�ۦP�Ϊ̤��P�����:
```js
    function NavController($scope){
        $scope.doSomething = doA;
    }
    
    function ContentAreaController($scope){
        $scope.doSomething = doB;
    }    
```
�o��, `doA()`�M`doB()`��ƥi��ɬۦP�Ϊ̤��P��, ���M��A�����̪��w�q.

�{�b�ڭ��ٳѤU��5�I, �X�ֵ��c�M�欰. �o�O�@�Ӧ���ĳ�����D, �]���A������X����t�������G, �����P�ڭ̤j���̩ҷQ���X�֪�{¾�d�M���ε{���޿誺�欰�D�`����. ��H�̽ͤ�����аO���c�M�欰�������ɭ�, �o��M�|���t�����v�T.

�p�G�ڭ̪��t�έ��{�o�ؽ��X���D��, �o�̦��@��²�檺���եi�H���U�ڭ̧�X��: �ڭ̥i�H���ڭ̪����ε{���޿�إߤ@�ӳ椸����, �Ӥ��ݭnDOM���s�b.

�bAngular��, �O��, �ڭ̥i�H�b������u�s�g�]�t�~���޿誺�N�X�Ӥ����ޥ�DOM. �b�ڭ̤��e�s�g��JavaScript��, �o�Ӱ��D�b�ƥ�B�z�{�Ǥ��O���s�b��. �`�N, �b�o�̥H�Φb�o���Ѫ���L�a��, �ثe�ڭ̩ҽs�g�������, ���S���ޥ�DOM�M����DOM�ƥ�B�z�{��. �A�i�H�ܻ��P�إߥX�o�Ǥ��aDOM�����. �Ҧ��������w��M�ƥ�B�z�{�ǳ��o�ͦbAngular��.

���o�Ӱ��D�b�s�g�椸���ծ�. �p�G�A�ݭnDOM, �A�b���դ��إߥ�, �u�|�W�[���յ{�Ǫ�������. ��A�������o���ܤƮ�, �A�ݭn�b�A�����դ�����DOM, �o�˥u�|�a�ӧ�h�����@�u�@. �̫�, �X��DOM�O�ܺC��, ���սw�C�N���ۤ��X���|�ήɥH�γ̲׸ѪR���O�w�C��. Angular��������ըèS���o�ǰ��D. 

�]���A�i�H�ܻ��P���n���ƥ�B�z�{�Ǫ�²��ʩM�iŪ��, �@�L�o�c�P���H�ϳ̨ι��.

###�C��, ���M��L���ƪ�����

�̦��Υi��N�OAngular���O, `ng-repeat`��󶰦X�����C�@�����إߤ@���@�դ������@���ƥ�. �A���Ӧb�A�Q�إߦC����D������a��ϥΥ�.

��p���ڭ̵��Ѯv�s�g�@�Ӿǥͪ�W�U�����ε{��. �ڭ̥i��q���A����o�ǥͪ����, ���O�b�o�ӨҤl��, �ڭ̥u�bJavaScript�N���w�q���@�Ӽҫ�:
```js
    var students = [{name: 'Mary Contrary', id:'1'},
                    {name: 'Jack Sprat', id: '2'},
                    {name: 'Jill Hill', id: '3'}];
                    
    function StudentListController($scope){
        $scope.students = students;
    }
```
�ڭ̥i�H���U���o�˨���ܾǥͦC��:
```html
    <ul ng-controller="">
        <li ng-repeat="student in students">
            <a href="/student/view/{{student.id}}">{{student.name}}</a>
        </li>
    </ul>
```
`ng-repeat`�N�|�s�@���Ҥ��Ҧ�HTML���ƥ�, �]�A���Ҥ����F��. �o��, �ڭ̱N�ݨ�:

+ Mary Contrary
+ Jack Sprat
+ Jill Hill

���O�챵��*/student/view/1, /student/view/2, /student/view/3*.

���p�ڭ̤��e�Ҩ�, ���ܾǥͼƲձN�|�۰ʧ��ܴ�V�C��. �p�G�ڭ̰��@�ǨҦp���J�@�ӷs���ǥͨ�C���Ʊ�:
```js
    var students = [{name: 'Mary Contrary', id:'1'},
                    {name: 'Jack Sprat', id: '2'},
                    {name: 'Jill Hill', id: '3'}];
                    
    function StudentListController($scope){
        $scope.students = students;
        
        $scope.insertTom = function(){
            $scope.students.splice(1, 0, {name: 'Tom Thumb', id: '4'});
        };
    }
```
�M��b�˪O���K�[�@�ӫ��s�өI�s:
```html
    <ul ng-controller="">
        <li ng-repeat="student in students">
            <a href="/student/view/{{student.id}}">{{student.name}}</a>
        </li>
    </ul>
    <button ng-click="insertTom()">Insert</button>
```
�{�b�ڭ̥i�H�ݨ�:

+ Mary Contrary
+ Tom Thumb
+ Jack Sprat
+ Jill Hill

`ng-repeat`���O�ٸg��`$index`���A���ѤF��e����������, �p�G�O���X���Ĥ@�Ӥ���, �������Y�Ӥ���, �Ϊ̬O�̫�@�Ӥ����ϥ�`$first`, `$middle`�M`$last`�|���A���Ѥ@�ӥ�����.

�A�i�H�Q���ϥ�`$index`�ӼаO��椤����. ���w�@�ӳo�˪��˪O:
```html
    <table ng-controller="AlbumController">
        <tr ng-repeat="track in album">
            <td>{{$index + 1}}</td>
            <td>{{track.name}}</td>
            <td>{{track.duration}}</td>
        </tr>
    </table>
```
�o�O���:
```js
    var album = [{name: 'Southwest Serenade', duration: '2:34'},
                 {name: 'Northern Light Waltz', duration: '3:21'},
                 {name: 'Eastern Tango', duration: '17:45'}];
                 
    function AlbumController($scope){
        $scope.album = album;
    };
```
�ڭ̱o��p�U���G:

1. Southwest Serenade     2:34
2. Northern Light Waltz   3:21
3. Eastern Tango         17:45

###���ûP���

�����, �W�U��ӷP���u��[*���:context-sensitive tools*]�H�Ψ�L�\�h���p, ��ܩM���ä����O�@�����䪺�S��. ���p�bAngular��, �ڭ̰��ҫ����ܤ�Ĳ�oUI������, �H�θg�ѫ��O�N���ܤϬM��UI��. 

�o��, `ng-show`�M`ng-hide`�Ω�B�z�o�Ǥu�@. ���̰��ǻ������̪���F��������ܩM���ê��\��. �Y, ��A�ǻ�����F����true��`ng-show`�N��ܤ���, ��false�ɫh���ä���. ���F����true��`ng-hide`���ä���, ��false����ܤ���. �o���M��A�ϥέ��ӧ���F���A�N��.

�o�ǫ��O�g�ѾA���]�w�������˦���`display: block`����ܤ���, �]�w�˦���`display: none`�����ä���. ���ڭ̬ݥH�ӥ��b�c�ت�Death Ray����O���������Ҥl:
```html
    <div ng-controller="DeathrayMenuController">
        <p><button ng-click="toggleMenu()">Toggle Menu</button></p>
        <ul ng-show="menuState.show">
            <li ng-click="stun()">Stun</li>
            <li ng-click="disintegrate()">Disintegrate</li>
            <li ng-click="erase()">Erase from history</li>
        </ul>
    </div>
```
```js
    function DeathrayMenuController($scope){
        $scope.menuState.show = false;
        
        $scope.toggleMenu = function(){
            $scope.menuState.show = !$scope.menuState.show;
        };
        
        // death ray functions left as exercise to reader
    };
```
###CSS���M�˦�

��ө���, �{�b�A�i�H�b�A�����ε{�����g�Ѩϥ�{{ }}���ȲŸ��j�w��ƪ��覡�ʺA���]�w���M�˦�. �ƦܧA�i�H�b�A�����ε{�����զ��ǰt�����W. �Ҧp, �A�Q�ھڱ���T�Τ@�ǿ��, �A�i�H���U���o�˱q��ı�W��ܵ��Τ�.

���p�UCSS:
```css
    .menu-disabled-true {
        color: gray;
    }
```
�A�i�H�ϥΤU�����˪O�b�A��DeathRay����`stun`��ƨӸT�άY�Ǥ���:
```html
    <div ng-controller="DeatrayMenuController">
        <ul>
            <li class="menu-disabled-{{isDisabled}}" ng-click="stun()">Stun</li>
            ...
        </ul>
    </div>
```
�A�i�H�g�ѱ���A���]�w`isDisabled`�ݩʪ���:
```js
    function DeathrayMenuController($scope){
        $scope.isDisabled = false;
        
        $scope.stun = function(){
            //stun the target, then disable menu to allow regeneration
            $scope.isDisabled = 'true';
        };
    }
```
`stun`��涵��class�N�]�w��`menu-disabled-`�[`$scope.isDisabled`����. �]������l�Ƭ�false, �q�{���p�U���G��`menu-disabled-false`. �Ӧ��ɳo�̨S���PCSS�W�h�ǰt������, �h�S���ĪG. ��`$scope.isDisabled`�]�w��true��, CSS�W�h�N�ܦ�`menu-disabled-true`, ���ɫh�I�s�W�h�Ϥ�r���Ǧ�.

�o�ا޳N�]�P�˾A�Ω�O�J���p�˦�, �Ҧp`style="{{some expression}}"`.

���M�Q�k�ܦn, ���O�o�̦��@�ӯ��I�N�O���ϥΤF�@�Ӥ������νu�ӲզX�A�����W. ���M�b�o�ӨҤl���ܮe���z��, ���O���i��ܧִN�|�ܱo���H�޲z, �A�������_���\Ū�A���˪O�MJavaScript�ӥ��T���إߧA��CSS�W�h.

�]��, Angular���ѤF`ng-class`�M`ng-style`���O. ���̳������@�Ӫ�F��. �o�Ӫ�F�����p�⵲�G�i�H�O�U�C���@:

+ �@�ӨϥΪŮ�������W���r�Ŧ�
+ �@�����W�Ʋ�
+ ���W�쥬���Ȫ��M�g

���ڭ̷Q���@�U, �A�Ʊ�b���ε{���Y�����@�ӼзǦ�m��ܿ��~�Mĵ�i���Τ�. �ϥ�`ng-class`���O, �A�i�H�o�˰�:
```css
    .error {
        background-color: red;
    }
    .warning {
        background-color: yellow;
    }
```
```html
    <div ng-controller="HeaderController">
        ...
        <div ng-class="{error: isError, warning: isWarning}">{{messageText}}</div>
        ...
        <button ng-click="showError()">Simulate Error</button>
        <button ng-click="showWarning()">Simulate Warning</button>
    </div>
```
```js
    function HeaderController($scope){
        $scope.isError = false;
        $scope.isWarning = false;
        
        $scope.showError = function(){
            $scope.messageText = 'This is an error';
            $scope.isError = true;
            $scope.isWarning = false;
        };
        
        $scope.showWarning = function(){
            $scope.messageText = 'Just a warning. Please carry on';
            $scope.isWarning = true;
            $scope.isError = false;
        };
    }
```
�A�Ʀܥi�H���X��}�G���Ʊ�, �Ҧp���G��椤�襤����. ��軡, �ڭ̭n�c�ؤ@���\�U�ؿ��åB�Ʊ氪�G�Τ��I��������.

�bCSS��, �ڭ̳]�w�@�Ӱ��G�檺�˦�:
```css
    .selected {
        background-color: lightgreen;
    }
```
�b�Ҫ���, �ڭ̳]�w`ng-class`��`{selected: $index==selectedRow}`. ��ҫ�����`selectedRow`�ݩʤǰtng-repeat��`$index`�ɳ]�wclass��selected. �ڭ��ٳ]�w�@��`ng-click`�ӳq������Τ��I���F���@��:
```html
    <table ng-controller="RestaurantTableController">
        <tr ng-repeat="restaurant in directory" ng-click="selectRestaurant($index)" ng-class="{selected: $index==selectedRow">
            <td>{{restaurant.name}}</td>
            <td>{{restaurant.cuisine}}</td>
        </tr>
    </table>
```
�b�ڭ̪�JavaScript��, �ڭ̥u�]�w�������\�U�M�إ�`selectRow`���:
```js
    function RestuarantTableController($scope){
        $scope.directory = [{name: 'The Handsome Heifer', cuisine: 'BBQ'},
                            {name: 'Green\'s Green Greens', cuisine: 'Salads'},
                            {name: 'House of Fine Fish', cuisine: 'Seafood'}];
        $scope.selectRestaurant = function(row){
            $scope.selectedRow = row;
        };
    }
```
###`src`�M`href`�ݩʪ`�N�ƶ�

����ô�����@��`<img>`�Ϊ�`<a>`���Ү�, ���W���@�˦b`src`�Ϊ�`href`�ݩʤ��ϥ�{{ }}�B�z���|�N�L�k���`�u�@. �]���b�s�������Ϥ��P��L���e�O�æ�[����, �ҥHAngular�L�k�d�I���ô�����ШD.

���`<img>`�Ө��̩��㪺�y�k�K�O:
```html
    <img src="/images/cats/{{favoriteCat}}">
```
�ۤ�, �A���Өϥ�`ng-src`�ݩʨù��U���o�˽s�g�A���˪O:
```html
    <img ng-src="/images/cats/{{favoriteCat}}">
```
�P�˪��D�z, ���`<a>`���ҧA���Өϥ�`ng-href`:
```html
    <a ng-href="/shop/category={{numberOfBalloons}}">some text</a>
```
###��F��

��F���I�᪺��Q�O���A�������b�A���˪O, ���ε{���޿�H�θ�Ƥ����إ߹_�l�ӻP���P�ɨ������ε{���޿谽���N�N���i�J�Ҫ���.

����{�b, �ڭ̤@���D�n�O�ޥέ�ͪ���Ƨ@����F���ǻ���Angular���O. ���O���o�Ǫ�F���i�H����h���Ʊ�. �A�i�H�B�z²�檺�ƾǹB��(+, -, /, *, %), �i����(==, !=, >, <, >=, <=), ���楬���޿�B��(&&, !!, !)�H�Ϋ���B��(\^, &, |). �A�i�H�I�s���S�b�����`$scope`�ﹳ�W�����, �A�٥i�H�ޥθ�ƩM�ﹳ��ܪk([], {}, �K).

�U�����O���Ī�F�����Ҥl:
```html
    <div ng-controller="SomeController">
        <div>{{recompute() / 10}}<div>
        <ul ng-repeat="thing in things">
            <li ng-class="{highlight: $index % 4 >= threshold($index)}">
                {{otherFunction($index)}}
            </li>
        </ul>
    </div>
```
�o�̪��Ĥ@�Ӫ�F��`recompute() / 10`�O���Ī�, �O�b�˪O���]�w�޿�ܦn���n�Ҥl, ���O�����קK�o�ؤ覡. �O�����ϩM���������¾�d�����i�H�T�O���̮e���z�ѩM����.

���M�A�i�H�ϥΪ�F�����ܦh�Ʊ�, ���̥�Angular�۩w�q�������������p��. �L�̨ä��ϥ�JavaScript��`eval()`����, eval()���۷�h������.

�ۤ�, ���̨ϥ�Angular�۱a���۩w�q����������. �b�̭�, �A���|�ݨ�`�����c(for, while����), �y�{����y�y(if-else, throw)�Ϊ̧��ܸ�ƪ��B���(++, --). ��A�ݭn�ϥγo���������B���, �A���Ӧb�A��������ϥΫ��O�i��B�z.

���ު�F���b�ܦh�譱��JavaScript��[�Y��, �����̹�`undefined`�M`null`�ä��O���Y��(��e�P). �˪O�u�O²�檺��V�@�ǪF��, �ä��|�ߥX�@��`NullPointerException`�����~. �o�˴N���\�A�w�����ϥμҫ��ӨS������, �åB�u�n���̱o���ƶ�R�N�����̥X�{�b�Τ�ɭ���.

###�����Τ�ɭ�(UI)�M���¾�d

�b�A�����ε{����������T��¾�d:

+ �b�A�����ε{�����ҫ����]�w��ժ��A.[��l�����ε{��]
+ �g��`$scope`���S�ҫ��M��ƨ���Ϥ�.
+ �ʱ��ҫ������ܨ�Ĳ�o�欰.

���Ĥ@�I�ĤG�I�b�������w�g�ݹL��h�Ҥl. �y�ԧڭ̷|�Q�׳̫�@�I. �M��, ����䷧���W���ت�, �O���ѥN�X�Ϊ̰���Τ�P���ϥ椬�@�檺�޿�. 

���F�O��������p���M����޲z, �ڭ̫�ĳ�A�w����Ϫ��C�@�Ӱϰ�إߤ@�ӱ��. �]�N�O��, �p�G�A���@�ӿ��h�إߤ@��`MenuController`. �p�G�A���@���ѥ]�h�ɯ�, �h�s�g�@��`BreadcrumbController`, ����.

�A�i��}�l���F, ���O�ݭn���T���N����j�w��@�ӫ��w��DOM�����Ω�޲z����. ����إD�n���覡���p����PDOM�`�I, �@�ؤ覡�O�b�˪O�����w�@��`ng-controller`�ݩ�, �t�@�ؤ覡�O�g��`route`(����)���p�@�ӰʺA�[����DOM�˪O���q, �]�٧@����.

�ڭ̱N�b�������᭱�A�Q��������ϩM���Ѫ��T��.

�p�G�A��UI�����@�ӽ��������q, �A�i�H�g�ѫإߴO�M�����, �g���~�Ӿ�Ӧ@�ɼҫ��M��ƨӫO���A���N�X�����ʩM�i���@��. �O�M�����²��, �A�i�H²�檺�b�t�@��DOM�����t�@�ӱ����@��DOM����������o�@�I, �N���o��:
```html
    <div ng-controller="ParentController">
        <div ng-controller="ChildController">�K</div>
    </div>
```
���M�ڭ̱N�o�Ӫ�F������O�M, ��ڪ��O�M�o�ͦb�@�ΰ줤($scope�ﹳ��). �ǻ����O�M�����`$scope`�~�Ӧۤ������`$scope`�쫬, �o�N���۶ǻ���`ChildController`��`$scope`�N���v�X�ݶǻ���`ParentController`��`$scope`���Ҧ��ݩ�.

###�ϥΧ@�ΰ�o�G�ҫ����

�N`$scope`�ﹳ�ǻ����ڭ̪�����K�O�ڭ̱N�ҫ���Ƽ��S�����Ϫ�����. �i��A�����ε{�����٦���L�����, ��Angular���u����g��scope�X�ݥ��i�H�X�ݪ��ҫ��������ݩ�. �A�i�H�{��scope�N�O�@���@�ӤW�U�����ҥΩ�b�A���ҫ����[���ܤƪ�.

�ڭ̤w�g�ݹL�F�ܦh���T�]�w�@�ΰ쪺�Ҥl, �N��`$scope.count = 5`. �]���@�Ƕ�������k�b�˪O���]�w��ۨ����ҫ�. �A�i�H���U���o�˰�:

1. �g�Ѫ�F��. �ѩ��F���B��b������@�ΰ����p���������W�U�夤, �b��F�����]�w�ݩʻP�b������@�ΰ줤�]�w�@���ݩʤ@��. 

�]�N�O���o��:  
```html
    <button ng-click="count=3">Set count to three</button>
```
�o�˰��]���ۦP���ĪG:
```html
    <div ng-controller="CountController">
        <button ng-click="setCount()">Set count to three</button>
    </div>
```
CountController�w�q�p�U:
```js
    function CountController($scope){
        $scope.setCount = function(){
            $scope.count = 3;
        }
    }
```
2. �b��檺��J�ؤ��ϥ�`ng-model`. �b��F����, �ҫ��Q���w��`ng-model`���ѼƤ]�A�Ω󱱨�@�ΰ�d��. ���~, �o�N�b���r�q�M�A���w���ҫ������إߤ@�����V���ô��.

###�ϥ�$watch�ʱ��ҫ��ܤ�

�Ҧ�scope��Ƥ��̱`�Ϊ��i��N�O$watch�F, ��A���ҫ������o���ܤƮɥ��|�q���A. �A�i�H�ʱ���ӹ�H�ݩ�, �]�i�H�ʱ��p�⵲�G(���), �X�G�Ҧ����ƪ����i��@�@���ݩʩΪ̤@��JavaScript�B�����Q�X��. �Ө�ƪ�ñ�W�p�U:
```js
    $watch(watchFn, watchAction, deepWatch);
```
�C�ӰѼƪ��ԲӰT���p�U:

**watchFn**

> �o�ӰѼƬO�@��Angular�r�Ŧ��F���Ϊ̬O�@�Ӫ�^�A�ҧƱ�ʱ����ҫ���e�Ȫ����. �o�Ӫ�F���|�Q�h������, �]���A�ݭn�T�O�����|���Ƨ@��. �]�N�O��, ���i�H�Q�I�s�h���Ӥ����ܪ��A. �P�˪���], �ʱ���F���]���ӬO�B������קC��(����²�檺�B��). �p�G�A�ǻ��@�Ӧr�Ŧꪺ��F��, ���N�|���I�s��(���檺��F��)�@�ΰ줤�����Ĺﹳ�D��.

**watchAction**

> �o�O`watchFn`�c���ܤƮɷ|�Q�I�s����ƩΪ̪�F��. �b��ƧΦ���, ������`watchFn`���s��, �­ȥH�Χ@�ΰ쪺�ޥ�. ��ñ�W�N�O`function(newValue, oldValue, scope)`.

**deepWatch**

> �p�G�]�w��true, �o�ӥi�諸�����ѼƥΩ�i�DAngular�ˬd�Һʱ�����H���C�@���ݩʪ��ܤ�. �p�G�A�Ʊ�ʱ��Ʋժ��ӧO�����Ϊ̹�H���ݩʦӤ��O�@�Ӵ��q����, ����A���ӨϥΥ�. �ѩ�Angular�ݭn�M���ƲթΪ̹ﹳ, �p�G���X(�Ʋդ���/�ﹳ����)�ܤj, ����p�⪺�N���|�D�`��.

��A���A�Q�����ܤƳq����, `$watch`��ƱN��^�@�ӵ��P��ť�������.

�p�G�ڭ̹��ʱ��@���ݩ�, �M��b�y����P��, �ڭ̱N�ϥΤU�����覡:
```js
    ...
    var dereg = $scope.$watch('someModel.someProperty', callbackOnChange);
    ...
    dereg();
```
���ڭ̦^�U�@�U�Ĥ@�������㪺�ʪ����d��. ��軡, ��Τ�b�L���ʪ������K�[�F�W�X100�������ӫ~��, �ڭ̧Ʊ�ӽ�10�������u�f. �ڭ̨ϥΤU�����˪O:
```html
    <div ng-controller="CartController">
        <div ng-repeat="item in items">
            <span>{{item.title}}</span>
            <input ng-model="item.quantity">
            <span>{{item.price | currency}}</span>
            <span>{{item.price * item.quantity | currency}}</span>
        </div>
        <div>Total: {{totalCart() | currency}}</div>
        <div>Discount: {{bill.discount | currency}}</div>
        <div>Subtotal: {{subtotal() | currency}}</div>
    </div>
```
�򱵵۬O`CartController`, ���ݰ_�ӹ��U���o��:
```js
    function CartController($scope){
        $scope.bill = {};

        $scope.items = [
            {title: 'Paint pots', quantity: 8, price: 3.95},
            {title: 'Polka dots', quantity: 17, price: 12.95},
            {title: 'Pebbles', quantity: 5, price: 6.95}
        ];

        $scope.totalCart = function(){
            var total = 0;
            for (var i = 0, len = $scope.items.length; i < len; i++){
                total = total + $scope.items[i].price* $scope.items[i].quantity;
            }

            return total;
        };

        $scope.subtotal = function(){
            return $scope.totalCart() - $scope.discount;
        };

        function calculateDiscount(newValue, oldValue, scope){
            $scope.bill.discount = newValue > 100 ? 10 : 0;
        }

        $scope.$watch($scope.totalCart, calculateDiscount);
    }
```
�`�N`CartController`������, �ڭ̵��Ω�p����ʶR�ӫ~�`����`totalCart()`���ȳ]�w�F�@�Ӻʱ�. �C��o�ӭ��ܤƮ�, �ʱ����|�I�s`calculateDiscount()`, �åB�|��discount(�u�f��)�]�w�@�ӾA����. �p�G�`����$100, �ڭ̱N�]�w�u�f��$10. �_�h, �u�f�N��$0.

�A�i�H�ݨ�o�Ӯi�ܵ��Τ᪺�Ҥl�p��2-1�ҥ�:

![use-$watch](figure/watch1.png)

��2-1 Shopping cart with discount

###watch()�����ʯ�`�N�ƶ�

�e���Ҥl�|���T������, ���O�o�̦��@�Ӽ�b���ʯ���D. ���M�ä�����, �p�G�A�b`totalCart()`���]�w�@�Ӱ����_�I, �A�|�o�{�b��V�����ɥ��Q�I�s�F6��. ���M�b�o�����ε{�����A�q�ӨS���`�N�쥦, ���O�b��h���������ε{����, �B�楦6���i��O�@�Ӱ��D.

������O6��? �䤤3���ڭ̥i�H�ܻ��������ܨ�, �]�������O�b�U���T�ӹL�{���B��@��:

+ �b`{{totalCart() | currency}}`�˪O��
+ `subtotal()`��Ƥ�
+ `$watch()`��Ƥ�

�M��OAngular�A�B�楦�̤@��, �]�ӱa���ڭ�6���B��. Angular�o�˰��O���F���Ҧb�A���ҫ����ܤƬO�_�����Ǽ��X�h�H�����ҧA���ҫ��O�_í�w. Angular�g���ˬd�@���Һʱ��ݩʪ��ƥ��P���̷�e�Ȥ���ӽT�{���̬O�_����. �ƹ�W, Angular�]�i�H�B�楦�h�F�Q���ӽT�O�O�_�����Ǽ��}. �p�G�o�ͳo�ر��p, �A�i��ݭn�̿�`���ӭ״_��.

���M�A�{�b�|��߳o�Ӱ��D, ���O��A�\Ū�����Ѯɥ��i��N���A�O���D�F. �M��Angular���o���bJavaScript����{���ô��, �ڭ̤@���PTC39���H�@�P�V�O��{�@�ө��h����ͪ�`Object.observe()`. �@�����F��, Angular�N�۰ʨϥ�`Object.observe()`�H���H�a�e�{���A�@�ӭ�ͮĲv�����ô��.

> Ķ�`: [TC39](http://www.ecma-international.org/memento/TC39.htm)

�b�U�@�����A�|�ݨ�, Angular���@�ӫܦn��Chrome�����X�R�{��(Chrome����)Batarang, ���N�۰ʵ��A��X(���G)���Q�����ô��(�q�ʯ઺���צӨ�, ��ܸ��ô�����覡�ä��O���n���覡).

> Ķ�`:
> 
> + [Batarang](https://chrome.google.com/webstore/detail/ighdmehidhipcmcojjgiloacoafjmpfk) - �o�O�@��Angular�����P�ʯ�ʱ��u��.
> + [Batarang-Github](https://github.com/angular/angularjs-batarang)

�{�b�ڭ̪��D�F�o�Ӱ��D, �o�̦��@�Ǥ�k�i�H�ѨM��. �@�ؤ覡�O�bitems�Ʋ��ܤƮɫإ�`$watch`�åB�u���s�p`$scope`��total, discount�Msubtotal�ݩʭ�.

����o�@�I, �ڭ̥u�ݭn�ϥγo���ݩʧ�s�˪O:
```html
    <div>Total: {{bill.total | currency}}</div>
    <div>Discount: {{bill.discount | currency}}</div>
    <div>Subtotal: {{bill.subtotal | currency}}</div>
```
�M��, �bJavaScript��, �ڭ̭n�ʱ�items�Ʋ�, �H�ΩI�s�@�Ө�ƨӭp��Ʋե��N���ܪ��`��:
```js
    function CartController($scope){
        $scope.bill = {};
        
        $scope.items = [
            {title: 'Paint pots', quantity: 8, price: 3.95},
            {title: 'Polka dots', quantity: 17, price: 12.95},
            {title: 'Pebbles', quantity: 5, price: 6.95}
        ];
        
        var calculateTotals = function(){
            var total = 0;
            for(var i = 0, len = $scope.items.length; i < len; i++){
                total = total + $scope.items[i].price * $scope.items[i].quantity;
            }
            
            $scope.bill.totalCart = total;
            $scope.bill.discount = total > 100 ? 10 : 0;
            $scope.bill.subtotal = total - $scope.bill.discount;
        };
        
        $scope.$watch('items', calculateTotals, true);
    }
```
�`�N�o��`$watch`���w�F�@��`items`�r�Ŧ�. �o�i��O�]��`$watch`��ƥi�H�����@�Ө��(���p�ڭ̤��e����)�Ϊ̤@�Ӧr�Ŧ�. �p�G�ǻ��@�Ӧr�Ŧ굹`$watch`���, �b`$scope`�I�s���@�ΰ줤���N�Q��@�@�Ӫ�F��.

�o�ش������b�A�����ε{�����i��u�@�o�ܦn. �M��, �ѧںʱ����Oitems�Ʋ�, Angular�N�|�s�@�@�Ӱƥ��H�ѧڭ̶i����. ���@�Ӹ��j��items�M��, �p�G�ڭ̦bAngular�C�@���p�⭶�����G�ɥu���s�p��bill�ݩʭ�, ���i���{�o��n. �ڭ̥i�H�g�ѫإߤ@��`$watch`�Ӱ���o�@�I, ���a���u�Ω󭫷s�p���ݩʪ�`watchFn`���. �N���o��:
```js
    $scope.$watch(function(){
        var total = 0;
        for(var i = 0, i < $scope.items.length; i++){
            total = total + $scope.items[i].price * $scope.items[i].quantity;
        };
        
        $scope.bill.totalCart = total;
        $scope.bill.discount = total > 100 ? 10 : 0;
        $scope.bill.subtotal = total - $scope.bill.discount;
    });
```
####�h�Ӻʱ�

�p�G�A�Q�ʱ��h���ݩʩΪ̹ﹳ, �åB�C���̵o�ͥ����ܤƮɳ�����@�Ө��. �A����Ӱ򥻪����:

+ �ʱ��ݩʯ��ޭ�.
+ �⥦�̩�J�ƲթΪ̹ﹳ�`�åB�N�ǻ���`deepWatch`�]�w��true.

> Ķ�`: ��夤��ӿﶵ�ƦC�����A��. Ķ�夤�ȥ��F���Ǩõ��X�������T��.

�b�Ĥ@�ر��p�U, �p�G�@�ΰ줤���@�ӹﹳ�֦�����ݩ�`a`�M`b`, �åB�Ʊ�b�o���ܤƮɰ���`callMe()`���, �A���ӦP�ɺʱ�����, �N���o��:
```js
    $scope.$watch('things.a + things.b', callMe(�K));
```
��M, �ݩ�`a`�M`b`�i��b���P����H��, �u�n�A���w�A�]�i�H�s�@�o�ӦC��. �p�G�C��ܪ�, �A�i�����w�s�g�@�Ӫ�^���ޭȪ���ƦӤ��O�̾a�@���޿��F��.

�b�ĤG�ر��p�U, �A�i��Ʊ�ʱ�`things`�ﹳ�����Ҧ��ݩ�. �b�o�ر��p�U, �A�i�H�o�˰�:
```js
    $scope.$watch('things' calMe(�K), true);
```
�o��, �g�ѱN�ĤT�ӰѼƳ]�w��`true`�ӭn�DAngular�M��`things`��H���ݩʨæb���̵o�ͥ�����ܮɩI�s`callMe()`. �o�P�˾A�Ω�Ʋ�, �u�O�o�̬O�w��@�ӹﹳ.

##�ϥμҲղ�´�̿�

�b���󤣥��Z�����ε{����, �b�A���N�X��줤�˲M���p���´�\��¾�d�q�`���O�@���}��������. �ڭ̤w�g�ݨ�F����O�p�����ϼ˪O�����ڭ̴��Ѥ@�Ӧs����S���T��ƩM��ƪ��ϰ�. ���O�ڭ̦b���̦w�m������ε{��������L�N�X�O? �̩��㪺�覡�N�O�N���̩�m�b���������Ƥ�.

���p�����ε{���M�ثe�ڭ̩Ҩ��L���Ҥl�o���覡�u�@�o�ܦn, ���O�b��ڪ����ε{�����N�ܧ��ܱo���H�޲z. ����N������n�@���H�Χڭ̻ݭn������Ʊ����U����. ���̥i������z��, �]�i���������(���H���@).

�ޤJ�Ҳ�. �b�A�����ε{���\���, ���̴��ѤF�@�ز�´�̿઺�覡, �H�Τ@�ئ۸ѨM�̿઺����(�]�٬��̿�`�J[*�Ĥ@�����w�g���ФF����O�̿�`�J*]). �@�뱡�p�U, �ڭ̺٤����̿����Y�A��, ���̵��ڭ̪����ε{�����ѯS��A��.

��p, �p�G�b�ڭ̪��ʪ�����������ݭn�q���A�����o�@�ӥX�ⶵ�ئC��, �ڭ̻ݭn�@�ǹﹳ--���ڭ̺٤���`Items`--�`�N�o�̬O�q���A�����o������. �ϹL��, `Items`�ﹳ, �ݭn�@�Ǥ覡�g��XHR�Ϊ�WebSockets�P���A���W����Ʈw�q�H.

���A�μҲճB�z�ݰ_�ӹ��o��:
```js
    function ItemsViewController($scope){
        // �V���A���o�_�ШD
        ...
        
        // �i�JItems�ﹳ�ѪR�^��
        ...
        
        // �b$scope���]�wItems�ƲեH�K���ϥi�H��ܥ�
    }
```
�M�ӳo�T�����u�@, ���O���s�b�@�Ǽ�b�����D.

+ �p�G�@�Ǩ�L������ٻݭn�q���A�����o`Items`, ���ڭ̲{�b�n�ƻs�o�ӥN�X. �o�y���F���@���t��, �p�G�ڭ̲{�b�n�c�y�Ҧ��Ϊ̨�L���ܤ�, �ڭ̥����b�n�X�Ӧa���s�o�ӥN�X.
+ �Ҽ{���L�]��, �p���A������, �ѪR�����׵���, �o�]�O�������_����ﹳ¾�d�ɭ�����], �N�X�]�����\Ū.
+ ��o�q�N�X�i��椸����, �ڭ̻ݭn�@�x��ڹB�檺���A���Ϊ̨ϥ�XMLHttpRequest���ɤB��^�������. �B����A���i����ձN�ɭP���իܺC, �t�m���ܵh�W, ���q�`�i�ܤF���դ����H��. �ӥ��ɤB���覡�ѨM�F�t�שM�H�����D, ���O�o�N���ۧA�����O��b���դ��M�z���󤣩w�ﹳ, �o�˴N�a�ӤF�B�~�������שM�ܮz��, �]�������ϧA���w�ǽT���u�W��������Ʈ榡(�C��榡�ܤƮɳ��ݭn��s����).

���ҲթM�q���̭��̨��o���̿�`�J, �ڭ̴N�i�H�s�g��²�䪺���, ���o��:

    function ShoppingController($scope, Items){
        $scope.items = Items.query();
    }
        
�{�b�A�i��|�ݦۤv, '��M, �o�ݰ_�ӫܻ�, ���O�o��Items�q���̨�?'. �e�����N�X���]�ڭ̤w�g�w�q�F�@���A�Ȫ�`Items`.

�A�ȬO�@�ӳ�W����H(��ҹﹳ), �����楲�n�����ȨӤ�����ε{�����\��. Angular�۱a�F�ܦh�A��, �Ҧp`$location`, �Ω�P�s���������a�}�椬, `$route`, �Ω����m(URL)���ܤƤ�������, �H��`$http`�Ω�P���A���q�H.

�A�i�H�]���ӫإߧA�ۤv���A�ȥh�B�z���ε{���Ҧ����S�����. �b�ݭn���̮ɪA�ȥi�H�@�ɵ����󱱨. �]��, ��A�ݭn�󱱨�q�H�M�@�ɪ��A�ɨϥΥ��̬O�@�ӫܦn������. Angular�j�w���A�ȳ��H`$`�}�Y, �ҥH�A�]����R�W���̬�����A���w���F��, �o�O�@�ӫܦn���D�N, �H�קK�ϥ�`$`�}�Y�a�Ӫ��R�W�Ĭ���D.

�A�i�H�ϥμҲչ�H��API�өw�q�A��. �o�̦��T�Ө�ƥΩ�إ߳q�ΪA��, ���̳������P�h���������ʩM��O:
```html
<table>
    <thead>
        <tr>
            <th>Function</th>
            <th>�w�q(Defines)</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>provider(name, Object/constructor())</td>
            <td>�@�ӥi�t�m���A��, �a���������إ��޿�. �p�G�A�ǻ��@�ӹﹳ, �����Ӧ��@�ӦW��`$get`�����, �Ω��^�A�Ȫ����. �_�h, Angular�|���]�A�ǻ��F�@�Ӻc�y���, ��I�s���ɫإ߹��.</td>
        </tr>
        <tr>
            <td>factory(name, $get Function())</td>
            <td>�@�Ӥ��i�t�m���A�Ȥ]�a���������إ��޿�. �A���w�@�Ө��, ��I�s��, ��^�A�ȹ��. �A�i�H�{���o�M<code>provider(name, { $get: $getFunction()})</code>�@��</td>
        </tr>
        <tr>
            <td>service(name, constructor())</td>
            <td>�@�Ӥ��i�t�m���A��, ��إ��޿�²��. �N��<code>provider</code>���c�y��ƿﶵ, Angular�I�s���ӫإߪA�ȹ��.</td>
        </tr>                
    </tbody>
</table>
```
�ڭ̵y��A�Ӭ�`provider()`���t�m�ﶵ, �{�b�ڭ̥��Өϥ�`factory()`�Q�׫e����Items�Ҥl. �ڭ̥i�H���o�˽s�g�A��:
```js
    // Create a module to support our shopping views.
    var shoppingModule = angular.module('ShoppingModule', []);
    
    // Set up service factory to create our Items interface to the server-side database
    shoppingModule.factory('Items', function(){
        var items = {};
        items.query = function(){
            // In real apps, we'd pull this data from the server�K
            return [
                {title: 'Paint pots', description: 'Pots full of paint', price: 3.95},
                {title: 'Polka dots', description: 'Dots with polka', price: 2.95},
                {title: 'Pebbles', description: 'Just little rocks', price: 6.95}
            ];
        };
        
        return items;
    });
```
��Angular�إ�`ShoppingController`��, ���|�N`$scope`�M�ڭ̭�~�w�q���s��Items�A�ȶǻ��i��. �o�O�g�ѰѼƦW�٤ǰt������. �]�N�O��, Angular�|�ݨ�ڭ̪�`ShoppingController`�������ñ�W, �óq����(���)�o�{�@��Items�ﹳ. �ѩ�ڭ̩w�qItems���@�ӪA��, ���|���D�q���̨��o��.

�H�r�Ŧꪺ�Φ��d�߳o�Ǩ̿൲�G�N���ۧ@���Ѽƪ`�J����ƴN��������c�y��Ƥ@�ˬO���ǵL����. �ä��O�����o��:
```js
    function ShoppingController($scope, Items){...}    
```
�ڭ̤]�i�H�o�˽s�g:
```js
    function ShoppingController(Items, $scope){...}
```
�̵M�M�ڭ̩ҧƱ檺�\��@��.

���F�b�˪O���ϥΥ�, �ڭ̻ݭn�i�D`ng-app`���O�ڭ̪��ҲզW��, �N���U���o��:
```html
    <html ng-app="ShoppingModule">
```
���F�����o�ӨҤl, �ڭ̥i�H�o�˹�{�˪O����l����:
```html
    <body ng-controller="ShoppingController">
        <h1>Shop!</h1>
        <table>
            <tr ng-repeat="item in items">
                <td>{{item.title}}</td>
                <td>{{item.description}}</td>
                <td>{{item.price | currency}}</td>
            </tr>
        </table>
    </body>
```
���Ϊ���^���G�ݰ_�Ӧp��2-2�ҥ�:

![use-module](figure/useModule.png)

��2-2 Shop items

###�ڭ̻ݭn�h�ּҲ�?

�@���A�ȥ����i�H���̿����Y, Module API���\�A�b���̿त�w�q�̿����Y.

�b�j�h�����ε{����, �إߤ@�ӳ�@���ҲձN�Ҧ����N�X��J�䤤�ñN�Ҧ����̿�]��b�̭����H�ܦn���u�@. �p�G�A�ϥΨӦ۲ĤT��w���A�ȩΪ̫��O, ���̦۱a����ۨ����Ҳ�. �ѩ�A�����ε{���̿०��, �A�i�H�ޥΥ��̧@���A�����ε{�����̿�.

�|�ӨҤl, �p�G�A�n�]�t(��c��)�Ҳ�SnazzyUIWidgets�MSuperDataSync, ���ε{�����Ҳ��n���ݰ_�ӹ��o��:
```js
    var appMod = angular.module('app', ['SnazzyUIWidgets', 'SuperDataSync']);
```
##�ϥιL�o���榡�Ƹ��

�L�o�����\�A�b�˪O���ϥδ��Ȥ覡�n���p���ഫ��ƨ���ܵ��Τ�. �ϥιL�o�����y�k�p�U:

    {{expression | filterName : parameter1 : �K parameterN }}
    
�䤤��F���O���N��Angular��F��, `filterName`�O�A�Q�ϥΪ��L�o���W��, �L�o�����ѼƨϥΫ_������. �ѼƦۨ��]�i�H�O���N���Ī�Angular��F��.

Angular�۱a�F�X�ӹL�o��, ���ڭ̤w�g�ݨ쪺currency:

    {{12.9 | currency}}
    
�o�q�N�X��ܦp�U:

> $12.9

�A���ȭ���ϥθj�w���L�o��(Angular���m��), �A�i�H²�檺�s�g�A�ۤv���L�o��. �Ҧp, �p�G�ڭ̷Q�إߤ@�ӹL�o���������D�����r���j�g, �ڭ̥i�H���U���o�˰�:
```js
    var homeModule = angular.module('HomeModule', []);
    homeModule.filter('titleCase', function(){
        var titleCaseFilter = function(input){
            var words = input.split(' ');
            for(var i = 0; i < words.length; i++){
                words[i] = words[i].charAt(0).toUpperCase() + words[i].slice(1);
            }
            
            return words.join(' ');
        };
        return titleCaseFilter;
    });
```
���@�ӹ��o�˪��˪O:
```html
    <body ng-app="HomeModule" ng-controller="HomeController">
        <h1>{{pageHeading | titleCase}}</h1>
    </body>
```
�M��g�ѱ�����J`pageHeading`�@���@�Ӽҫ��ܼ�:
```js
    function HomeController($scope){
        $scope.pageHeading = 'behold the majesty of you page title';
    }
```
�ڭ̷|�ݨ�p��2-3�ҥܪ��F��:

![titleCase](figure/titleCase.png)

��2-3 Title case filter

##�ϥθ��ѩM$location��s����

����Ajax�q�޳N�W���O�歶���ε{��(�z�פW���̶ȶȦb�Ĥ@���ШD�ɥ[��HTML����, �M��u�ݦbDOM����s�϶�), �ڭ̳q�`�|���h�Ӥl�������ϥΩ�A����ܵ��Τ�Ϊ�����.

�ڭ̥i�H�ϥ�Angular��`$route`�A�Ȩӵ��ڭ̺޲z�o�ӳ���. ���A���w����, ����s�������V���w��URL, Angular�N�[������ܤ@�Ӽ˪O, �åB��ҤƤ@�ӱ�����˪O���ѤW�U������.

�g�ѩI�s`$routeProvider`�A�Ȫ��\��@���t�m���Ӧb�A�����ε{�����إߵ���. �N���o�˪����N�X:
```js
    var someModule = angular.module('someModule', [�K Module dependencies �K]);
    someModule.config(function($routeProvider){
        $routeProvider.
            when('url', {controller: aController, templateUrl: '/path/to/template'}).
            when(�Kother mappings for your app �K).
            �K 
            otherwise(�Kwhat to do if nothing else matches�K);
    });
```
�W�����N�X��ܷ��s������URL�ܤƬ����w��URL��, Angular�N�q`/path/to/template`���[���˪O, �èϥ�`aController`���p�o�Ӽ˪O���ڤ���(�N���ڭ̿�J`ng-controller=aController`).

�b�̫�@��I�s`otherwise()`�Ω�i�D���Ѧp�G�S����L���ǰt�h�������.

���ڭ̨ӨϥΤ@�U. �ڭ̥��b�c�ؤ@��email���ε{���N���P���Գ�Gmail, Hotmail�H�Ψ�L��. �ڭ̼ȥB�٥���A-mail. �{�b, ���ڭ̱q²�檺�}�l. �ڭ̪����̤���ܤ@�ӥ]�A���, ���D�H�εo�e�̪��l��T���C��. ��A�I���@�ӰT��, �����ӦV�N�l�󪺥���T����ܵ��A.

> �ѩ��s�������w������, �p�G�A�Q�ۤv���ճo�ǥN�X, �A�ݭn�b�@��Web�A�ȩ_�Ӷi��Ӥ��O�ϥ�`file://`. �p�G�A�w�ˤFPython, �A�i�H�b�A���u�@�ؿ��g�Ѱ���`python -m SimpleHTTPServer 8888`�Өϥγo�ǥN�X.

���D�˪O, �ڭ̷|���@�I���P���F��. �Ӥ��O�N�Ҧ����F�賣��b���̨ӥ[��, �ڭ̥u�|�إߤ@�ӥΩ��m���Ϫ����p�˪O. �ڭ̷|����b���Ϥ���m����, ��p���. �b�o�ر��p�U, �ڭ̥u�ݭn��ܤ@�Ӽ��D�]�t���Ϊ��W��. �M��ϥ�`ng-view`���O�ӧi�DAngular�ڭ̧Ʊ���ϥX�{�b����.

###*index.html*
```html
    <html ng-app="Amail">
        <head>
            <script src="js/angular.js"></script>
            <script src="js/controllers.js"></script>
        </head>
        <body>
            <h1>A-Mail</h1>
            <div ng-view></div>
        </body>
    </html>
```
�ѩ�ڭ̪����ϼ˪O�N�Q���J����إߪ��e����, �ڭ̥i�H�⥦�̽s�g���ϰ쪺HTML���. ���l��C��, �ڭ̱N�ϥ�`ng-repeat`�ӹM���T���C��ñN���̴�V��@�Ӫ�椤.

###*list.html*
```html
    <table>
        <tr>
            <td><strong>Sender</strong></td>
            <td><strong>Subject</strong></td>
            <td><strong>Date</string></td>
        </tr>
        <tr ng-repeat="message in messages">
            <td>{{message.sender}}</td>
            <td><a href='#/view/{{message.id}}'>{{message.subject}}</a></td>
            <td>{{message.date}}</td>
        </tr>
    </table>
```
�`�N�o�̧ڭ̥������Τ�g���I���D�D�N�L�ɯ��ԲӰT����. �ڭ̱NURL���ô����`message.id`�W, �]���I���@��`id=1`�������N�ϥΤ�����`/#/view/1`. �ڭ̱N�g��url�i��ɯ�, �]�٬��`���챵, �b�ԲӰT�����Ϫ������, ���S�w�����������@�ӸԱ�����.

���F�إ߮������Ա�����, �ڭ̱N�إߤ@����ܳ��message�ﹳ�ݩʪ��˪O.

###*detail.html*
```html
    <div><strong>Subject:</strong> {{message.subject}}</div>
    <div><strong>Sender:</strong> {{message.sender}}</div>
    <div><strong>Date:</strong> {{message.date}}</div>
    <div>
        <strong>To:</strong>
        <span ng-repeat="recipient in message.recipients">{{recipient}}</span>
    </div>
    <div>{{message.message}}</div>
    <a href="#/">Back to message list</a>
```
�{�b, �N�o�Ǽ˪O�P�@�Ǳ�����p�_��, �ڭ̱N�t�m`$routeProvider`�PURLs�өI�s����M�˪O.

###*controllers.js*
```js
    //Create a module for our core AMail services
    var aMailServices = angular.module('AMail', []);
    
    //Set up our mappings between URLs, tempaltes. and  controllers
    function emailRouteConfig($routeProvider){
        $routeProvider.
        when('/', {
            controller: ListController,
            templateUrl: 'list.html'
        }).
        // Notice that for the detail view, we specify a parameterized URL component by placing a colon in front of the id
        when('/view/:id', {
            controller: DetailController,
            templateUrl: 'detail.html'
        }).
        otherwise({
            redirectTo: '/'
        });
    };
    
    //Set up our route so the AMailservice can find it
    aMailServices.config(emailRouteConfig);
    
    //Some take emails
    messages = [{
        id: 0, sender: 'jean@somecompany.com',
        subject: 'Hi there, old friend',
        date: 'Dec 7, 2013 12:32:00',
        recipients: ['greg@somecompany.com'],
        message: 'Hey, we should get together for lunch somet ime and catch up. There are many things we should collaborate on this year.'
    },{
        id: 1, sender: 'maria@somecompany.com',
        subject : 'Where did you leave my laptop?' ,
        date: 'Dec 7, 2013 8:15:12',
        recipients: ['greg@somecompany.com'],
        message: 'I thought you were going to put it in my desk drawer. But i t does not seem to be there. '
    },{
        id: 2, sender: 'bill@somecompany.com',
        subject: 'Lost python',
        date: 'Dec 6, 2013 20:35:02',
        recipients: ['greg@somecompany.com'],
        message: "Nobody panic, but my pet python is missing from her cage. She doesn't move too fast, so just call me if you see her."
    }];

    // Publish our messages for the list template

    function ListController($scope){
        $scope.messages = messages;
    }

    //Get the message id fron the route (parsed from the URL) and use it to find the right message object.
    function DetailController($scope, $routeParams){
        $scope.message = messages[$routeParams.id];
    }
```
�ڭ̤w�g�إߤF�@�ӱa���h�ӵ��Ϫ����ε{�����򥻵��c. �ڭ̸g�ѧ���URL�Ӥ�������. �o�N���ۥΤ�]����ϥΫe�i�M��h���s�i��u�@. �Τ�i�H�b�ڭ̪����ε{�����K�[���ҩM�l���챵, �Y�ϥu���@�ӯu����HTML����.

##��ܦ��A��

�n�F, ���ܤֻ�. ��ڪ����ε{���q�`�P�u�������A���q�T. �������ΩM�s����Chrome�ୱ���ε{���i�঳�Ǩҥ~, ���O����L���@��, �A�O�_�Ʊ楦���[�O�s���ݩΪ̻P�Τ��ɥ椬, �A�i��Ʊ�A�����ε{���P���A���q�H.

���o�@�IAngular���ѤF�@�ӦW��`$http`���A��. �����@�ө⹳���s�x���C��ϱo������ܮe���P���A���q�H. ��������q��HTTP, JSONP�H��CORS. �٥]�A����JSON�|�}�MXSRF���w����ĳ. �����A�ܮe���ഫ�ШD�M��Ʀ^��, �Ʀ��ٹ�{�F²�檺�֨�. 

��軡, �ڭ̧Ʊ�q���A���˯��ʪ����I���ӫ~�Ӥ��O�ڭ̪����s������. �s�g���A�����T���W�X�F���Ѫ��d��, �]�����ڭ̷Q���@�U�ڭ̤w�g�إߤF�@�ӪA��, ��A�c�y�@��`/product`�d�߮�, ����^�@��JSON�Φ������~�C��.

���w�@�Ӧ^��, �ݰ_�ӹ��o��:
```json
    [
        {
            "id": 0,
            "title": "Paint pots",
            "description": "Pots full of paint",
            "price": 3.95
        },
        {
            "id": 1,
            "title": "Polka dots",
            "description": "Dots with that polka groove",
            "price": 12.95
        },
        {
            "id": 2,
            "title": "Pebbles",
            "description": "Just little rocks, really",
            "price": 6.95
        }
        �K etc �K     
    ]
```
�ڭ̥i�H�o�˽s�g�d��:
```js
    function ShoppingController($scope, $http){
        $http.get('/products').success(function(data, status, headers, config){
            $scope.items = data;
        });
    }
```
�M�ṳ�o�˦b�˪O���ϥΥ�:
```html
    <body ng-controller="ShoppingController">
        <h1>Shop!<h1>
        <table>
            <tr ng-repeat="item in items">
                <td>{{item.title}}</td>
                <td>{{item.description}}</td>
                <td>{{item.price | currency}}</td>
            </tr>
        </table>
    </body>
```
���p�ڭ̤��e�Ҿǲߨ쪺, �q�����Ӭݧڭ̱N�o���u�@�e�U����A���q�H�A�ȤW�i�H�󱱨�@�ɬO������. �ڭ̱N�b��5���Ӭݳo�ӵ��c�M����쪺�Q��`$http`���.

##�ϥΫ��O��sDOM

���O�X�RHTML�y�k, �]�O�N�欰�PDOM�ഫ���۩w�q�����M�ݩ����p�_�Ӫ��覡. �g�ѥ���, �A�i�H�إߴ_�Ϊ�UI�ե�, �t�m�A�����ε{��, ������A��Q��b�˪O���n�����Ʊ�.

�A�i�H�ϥ�Angular�۱a�����m���O�s�g����, ���O�A�i��|�Ʊ�B��A�ۤv�ҽs�g�����O�����p. ��A�Ʊ�B�z�s�����ƥ�M�ק�DOM��, �p�G�L�k�g�Ѥ��m���O���, �A�|���D�O�ɭԥ��}���O�W�h�F. �A�ҽs�g���N�X�b���O��, ���O�b�����, �A�Ȥ�, �]���O���ε{������L�a��.

�P�A�Ȥ@��, �g��module��H��API�I�s����`directive()`��ƨөw�q���O, �䤤`directiveFunction`�O�@�Ӥu�t��ƥΩ�w�q���O���\��(�S��).
```js
	var appModule = angular.module('appModule', [...]);
	appModule.directive('directiveName', directiveFunction);
```
�s�g���O�u�t��ƬO�ܲ`����, �]���b�o���Ѥ��ڭ̱M�����@�ӧ��㪺�@��. �Q�Q�A���G�f, ���L, �ڭ̥��Ӭݤ@��²�檺�Ҥl.

HTML5�����@�Ӱ��j���٬�`autofocus`���s�ݩ�, �N��L���J�I���@��input����. �A�i�H�ϥΥ����Τ�Ĥ@�ɶ��g�ѥL�̪���L�P�����椬�Ӥ��ݭn�I��. �o�O�ܦn��, �]�����i�H���A�n�����w�A�Ʊ��s����������ӵL�ݽs�g����JavaScript. ���O�p�G�A�Ʊ�N�J�I���@�ǫDinput�����W, ���챵�Ϊ̥���`div`�W�|���? �p�G�A�Ʊ楦�]��u�@�b�����HTML5���|���? �ڭ̥i�H�ϥΤ@�ӫ��O����o�@�I.
```js
	var appModule = angular.module('app', []);
	
	appModule.directive('ngbkFocus', function(){
		return {
			link: function(scope, elements, attrs, controller){
				element[0].focus();
			}
		};
	});
```
�o��, �ڭ̪�^���O�t�m�ﹳ�a�����w��link���. �o��link��ƨ��o�F�@�ӫʳ����@�ΰ�ޥ�, �@�ΰ줤��DOM����, �ǻ������O�����N�ݩʼƲ�, �H��DOM���������, �p�G���s�b. �o��, �ڭ̶ȶȥu�ݭn���o�����éI�s����`focus()`��k.

�M��ڭ̥i�H���o�˦b�@�ӨҤl���ϥΥ�:

###*index.html*
```html
	<html lang="en" ng-app="app">
		...include angular and other scripts...
		<body ng-controller="SomeController">
			<button ng-click="clickUnfocused()">
				Not focused
			</button>
			<button ngbk-focus ng-click="clickFocused()">
				I'm very focused!
			</button>
			<div>{{message.text}}</div>
		</body>
	</html>
```
###*controller.js*
```js
	function SomeController($scope) {
		$scope.message = { text: 'nothing clicked yet' };

		$scope.clickUnfocused = function() {
			$scope.message.text = 'unfocused button clicked';
		};

		$scope.clickFocused = function {
			$scope.message.text = 'focus button clicked';
		}
	}

	var appModule = angular.module('app', ['directives']);
```
����J������, �Τ�N�ݨ�аO��"I'm very focused!"���s�a�����G�J�I. �V���Ů���Ϊ̦^����N�ɭP�I���éI�s`ng-click`, �N�]�wdiv����r��"focus button clicked". �b�s���������}�o�ӭ���, �ڭ̱N�ݨ�p��2-4�ҥܪ��F��:

![foucsed](figure/custom-directive.png)

��2-4 Foucs directive

##���ҥΤ��J

Angular�a���X�ӾA�Ω�歶���ε{�����������\��Ӧ۰ʼW�j`<form>`����. �䤤���@�Ӥ������S�ʴN�OAngular���A�b��椺��input���n�����Ҫ��A, �ä��\�b��դ����g�����Ҫ����p�U�~����.

�Ҧp, �p�G�ڭ̫إߤ@�ӵn�����, �ڭ̥�����J�@�ӦW�٩Memail, ���O���@�ӥi�諸�~�֦r�q, �ڭ̥i�H�b�L�̴������A�����e���Ҧh�ӥΤ��J. �p�U�[���o�ӨҤl���s�������N��ܦp��2-5�ҥ�:

![valid](figure/signup.png)

��2-5. Form validation

�ڭ��٧Ʊ�T�O�Τ�b�W�٦r�q��J��r, ��J���T�Φ���email�a�}, �H�ΥL�i�H��J�@�Ӧ~��, ���~�O���Ī�.

�ڭ̥i�H�b�˪O������o�@�I, �ϥ�Angular��`<form>`�X�R�M�U��input����, �N���o��:
```html
	<h1>Sign Up</h1>
	<form name='addUserForm'>
		<div>First name: <input ng-model='user.first' required></div>
		<div>Last name: <input ng-model='user.last' required></div>
		<div>Email: <input type='email' ng-model='user.email' required></div>
		<div>Age: <input type='number' ng-model='user.age' ng-maxlength='3' ng-minlength='1'></div>
		<div><button>Submit</button></div>
	</form>
```
�`�N, �b�Y�Ǧr�q�W�ڭ̨ϥΤFHTML5����`required`�ݩʥH��`email`�M`number`������input�����ӳB�z�ڭ̪�����. �o���Angular�ӻ��O�ܦn��, �b�Ѧ��������HTML5���s����, Angular�N�ϥΧΦ��ۦP¾�d�����O.

�M��ڭ̥i�H�g�ѧ��ܤޥΥ����Φ��ӲK�[�@�ӱ���B�z��檺����.
```html
	<form name='addUserForm' ng-controller="AddUserController">
```
�b����̭�, �ڭ̥i�H�g�Ѥ@�Ӻ٬�`$valid`���ݩʨӳX�ݳo�Ӫ�檺���Ҫ��A. ��Ҧ������input�g�����Ҫ��ɭ�, Angular�N�]�w��($valid)��true. �ڭ̥i�H�ϥ�`$valid`�ݩʰ��@�Ǯɻ쪺�Ʊ�, ��p�����٨S�������ɸT�δ�����s.

�ڭ̥i�H�����洣��i�J�L�Ī��A, �g�ѵ�������s�K�[�@��`ng-disabled`.
```html
	<button ng-disabled='!addUserForm.$valid'>Submit</button>
```
�̫�, �ڭ̥i��Ʊ汱��i�D�Τ�o�w�g�K�[���\�F. �ڭ̪��̲׼˪O�ݰ_�ӹ��o��:
```html
	<h1>Sign Up</h1>
	<form name='addUserForm' ng-controller="AddUserController">
		<div ng-show='message'>{{message}}</div>
		<div>First name: <input name='firstName' ng-model='user.first' required></div>
		<div>Last name: <input ng-model='user.last' required></div>
		<div>Email: <input type='email' ng-model='user.email' required></div>
		<div>Age: <input type='number' ng-model='user.age' ng-maxlength='3'
		ng-min='1'></div>
		<div><button ng-click='addUser()'
		ng-disabled='!addUserForm.$valid'>Submit</button>
	</form>
```
���U�ӬO���:
```js
	function AddUserController($scope) {
		$scope.message = '';

		$scope.addUser = function () {
			// TODO for the reader: actually save user to database...
			$scope.message = 'Thanks, ' + $scope.user.first + ', we added you!';
		};
	}
```
##�p��

�b�e�⳹��, �ڭ̬ݨ�FAngular���Ҧ��̱`�Ϊ��\��(�S��). ��C�ӥ\�઺�Q��, �\�h�B�~���Ӹ`�T�����S���л\��. �b�U�@��, �ڭ̱N���A�g�Ѭ�s�@�Ө嫬���u�@�y�{�A�ѧ�h���T��.
