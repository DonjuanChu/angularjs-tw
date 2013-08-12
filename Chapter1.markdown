#�Ĥ@�� AngularJS²��

�ڭ̳гy��H�����Web�����ε{������O�O���i��ĳ��, ���O�إ߳o�����ε{���ɩүA�Ϊ������ʤ]�O���H���H�m�H��. �ڭ̪�Angular�ζ��Ʊ��ڭ̦b�ѻP�}�oAJAX���ε{���ɪ��h�W. �bGoogle, �ڭ̴��g�b�c�ع�Gmail, Maps, Calendar�H�Ψ�L�X�Ӥj��Web���ε{���ɸg���F�̵h�W���аV. �ڷQ�ڭ̤]�\����Q�γo�Ǹg������h���H���q.

�ڭ̧Ʊ�b�s�gWeb���ε{���ɷPı�󹳬O�Ĥ@���ڭ̽s�g�F�X��N�X�ï��b�᭱��Y�󥦵o�ͤF����. �ڭ̧Ʊ�s�X���L�{�Pı�󹳬O�гy�Ӥ��O���Ϻ���Web�s������_�Ǫ������B�@�u�@.

�P���P��, �ڭ��٧Ʊ����ү�����U�ڭ̧@�X�]�p���, �����ε{���ܮe���إߨñq�@�}�l�N�ܮe���z��, �åB�H�ۥ��̪����_����, ���T����ܷ|���ڭ̪����ε{���������, �X�R�M���@.

�ڭ̵��ϦbAngular������o��. �w�g���o�����G���ڭ̫D�`����. �o�ܤj�{�פW�k�\��Angular�}�����Ϥ����������X��u�@�M�ۤ����U, �P�ɤ]���ڭ̾ǲߨ��h���F��. �ڭ̧Ʊ�A�]�[�J��ڭ̪����Ϥ���, �����U�ڭ̧V�O��Angular�ܱo��n.

�A�i�H�b�ڭ̪�[Github�D��](https://github.com/shyamseshadri/angularjs-book)���ܮw���d�ݨ��Ǹ��j���Ϊ̸��������Ҥl�M�N�X���q, �A�]�i�H�Ԩ�����H�ά�s�o�ǥN�X.

##����

�b�A�N�ϥΪ�Angular���Τ����X�Ӯ֤ߪ�����. �ƹ�W, ����o�Ƿ����ä��O�ڭ̵o����. �ۤ�, �ڭ̱q��L�}�o���ҭ�ų�F�j�q���\�����k, �èϥΥ]�tHTML, �s�����M�\�h��LWeb�зǪ��覡��{�F��.

###�Ȥ�ݼ˪O

�h������Web���ε{�����O�g�Ѳո˩M�s�����A���W��ƨӫإ�HTML, �M��N�����������o�e���s������. �j�h�ƪ��歶���ε{�� - �]�٬�AJAX���ε{�� - �o�@�I�����ܦn, �b�Y�ص{�פW. Angular�H���P���覡�ո˼˪O�M��ƨñ��e���s�������B��.  �M����A���N�ܦ����˪O�����R�A�귽�M���o�Ǽ˪O���ѩһݪ����T��ƪ�����.

���ڭ̨Ӭݤ@�ӨҤl, �bAngular���p��b�s�������ո˼˪O�M���. �ڭ̷ӺD�ҨϥΤ@��Hello, World���Ҥl, ���O�ä��O�s�g�@��"Hello, World"����@�r�Ŧ�, �ӬO�c�y�o�Ӱݭ�"Hello"�@���y��ڭ̥i��|���ܪ����.

�w�復, �ڭ̫إߤF�@��`hello.html`�˪O:
```html
    <html ng-app>
    <head>
        <script src="angular.js"></script>
        <script src="controller.js"></script>
    </head>
    
    <body>
        <div ng-controller="HelloController">
            <p>{{greeting.text}}, World</p>
        </div>
    </body>
    </html>    
```
�M��ڭ̦b`controller.js`���s�g�޿�:
```js
    function HelloController($scope){
        $scope.greeting = {text: 'Hello'};
    }
```
�N`hello.html`���J���N�s������, �ڭ̱N�ݨ�p��1-1�ҥ�:

![Hello](figure/hello.png)

��1-1 Hello World

��{�b�ϥμs�x���j�h�Ƥ�k�ۤ�, �o�̦��@�Ǧ��쪺�Ʊ��ݭn�`�N:

+ HTML�èS�����Ϊ�ID�H�T�w�b���̲K�[�ƥ��ť��.
+ ��`HelloController`�]�w`greeting.text`��`Hello`��, �ڭ̨èS�����U����ƥ��ť���Ϊ̽s�g����^�I���.
+ `HelloController`�u�O�@�ӫܴ��q��JavaScript��, ���èS���~�ӥ���Angular���Ѫ��F��.
+ `HelloController`�����һݪ�`$scope`�ﹳ, �ӵL�ݫإߥ�.
+ �ڭ̨èS���I�sHelloController�ۨ����c�y��, �Ϊ̦b�I�s���ɨӭp�⥦.

���U�ӧڭ̷|�ݨ��h���t��, ���O�ڭ����ӲM��, Angular���ε{�������c�P�L�h���������ε{���������P.

������ڭ̧@�X�F�o�ǳ]�p��ܥH��Angular�O�p��u�@��? ���ڭ̨Ӭݬ�Angular�q��L�a���ų���@�Ӧn������.

###�ҫ�/����/���(MVC)

MVC���ε{�����c�O20�@��70�~�N�Q�@��Smalltalk���@�����޶i��. �qSmalltalk�}�l, MVC�b�X�G�C�@�ӯA�ΥΤ�ɭ����ୱ�}�o���Ҥ����ܱo���w��. �L�קA�O�ϥ�C++, Java�٬OObject-C, �����i�H�Q��MVC����. �M��, ����̪�, MVC�~�}�l���Ω�Web�}�o��. *[MVC was all but foreign to web development. �j�N: �X�G�PWeb�}�o��������]*

MVC�I�᪺�֤߫�Q�O�A�i�H�b�A���N�X�޲z���M�����������(�ҫ�), ���ε{���޿�(���)�H�ε��Τ�e�{���(����).

���ϱq�ҫ������o��ƨ���ܵ��Τ�. ��Τ�g���I���Ϊ̿�J�P���ε{���椬��, ����g�ѧ��ܼҫ�������ƨӦ^��. �̫�, �Ӽҫ��|�q�����ϥ��w�g�o�ͧ���. �H�K���i�H��s����ܪ��T��. 

�bAngular���ε{����, ���ϴN�O���ﹳ�ҫ�(DOM), ����OJavaScript��, �ҫ���Ʀs�x�b��H���ݩʤ�.

�ڭ̻{��MVC���F���D�n�O�H�U�X�ӭ�]. ����, �����A�b�����\�񤰻򴣨ѤF�@�Ӵ���ҫ�, �]���A���ݭn�C�����гy��. ��L�H�ѻP��A�����ؤ��X�@��, �N����Y�ɲz�ѧA�w�g�s�g�n������, �]���L�̷|���D�A�ϥΤFMVC���c�Ӳ�´�A���N�X. �]�\�̭��n���O, �����A�����ε{��������X�R, ���@�M���մ��ѤF���j���n�B.

**Ķ�`, �ѦҾ\Ū:** 

1. MVC�O�n��u�{�����@�سn��[�c�Ҧ� - [MVC](http://zh.wikipedia.org/wiki/MVC)
2. Smalltalk�O�@�����V��H���{�ǳ]�p�y�� - [Smalltalk](http://zh.wikipedia.org/wiki/Smalltalk)

###���ô��

���e�`����AJAX�歶���ε{��, ��Rails, PHP�Ϊ�JSP���x���O�b�g�Ѧb�o�e���Τ���ܤ��e�N��ƦX�֨�HTML�r�Ŧꤤ�����U�ڭ̫إߥΤ�ɭ�(UI).

��jQuery�o�˪��禡�w�]�O�N�ҫ��X�R��Ȥ�ݨ����ڭ̨ϥ�����������, ���O���u����W��s����DOM����O, �Ӥ����s��ӭ���. �o��, �ڭ̱N��ƦX�֨�r�Ŧ�Φ���HTML�˪O��, �M��g�Ѧb�@�Ӧ��줸�����]�w`innerHTML`�N��^�����G���J��ڭ̩ҧƱ檺DOM������.

�o�@�����u�@�o�ܦn, ���O��A�Ʊ洡�J�s����ƨ�Τ�ɭ�(UI)����, �Ϊ̰��Τ᪺��J���ܸ��, �A�ݭn���@�Ǭ۷����Z���u�@�H�T�O�A����ƪ��A���ǽT��, �L�׬O�b�Τ�ɭ���(UI)�٬OJavaScript�ݩʤ�.

���O�p�G�ڭ̥i�H���νs�g�N�X�N��B�z�n�o�@�Ǫ��u�@�|���? �p�G�ڭ̥i�H�u���n���Τ�ɭ������ǳ�������JavaScript�������ݩʨ������̦۰ʦP�B�S�|���? �o�ؽs�{����Q�٬����ô��. �ѩ󥦬OMVC���@�����j���u�{, �K��A�s�g���ϩM�ҫ��ɴ�֥N�X, �ڭ̧⥦�ޤJ��FAngular��. �j�����N��Ʊq�@�B�E����t�@�B���u�@���|�۰ʧ���.

�Ӭݬݳo�@�欰, ���ڭ̨ϥβĤ@�ӨҤl�������ʰ_��. ��ӬO, �@��HelloController�]�w�F��ҫ�`greeting.text`, ���K���A����. ���ڭ̸g�ѲK�[�@�ӮھڥΤ��J����`greeting.text`�Ȫ���r��J�بӧ��ܳo�ӨҤl, �����������.

�o�̬O�s���˪O:
```html
    <html ng-app>
    <head>
        <script src="angular.js"></script>
        <script src="controllers.js"></script>
    </head>
    
    <body>
        <div ng-controller="HelloController">
            <input ng-model="greeting.text" />
            <p>{{greeting.text}}, World</p>
        </div>
    </body>
    </html>
```
`HelloController`����i�H�O������.

�N�����J���s������, �ڭ̱N�ݨ�p��1-2�ҥܿù��I��:

![Hello with data binding](figure/hello2.png)

��1-2 ���ε{�����q�{���A

�p�G�ڭ̨ϥ�'Hi'��r������J�ؤ���'Hello', �ڭ̱N�ݨ�p��1-3�ҥܺI��:

![Hi](figure/hello3.png)

��1-3 ���ܤ�r�حȤ��᪺���ε{��

�ڭ̨èS���b��J�r�q�W���U���ܭȪ���ť��, �ڭ̦��@�ӱN�|�۰ʧ�s��UI.
�P�˪����p�]�A�Ω�Ӧۦ��A���ݪ�����. �b�ڭ̪������, �ڭ̥i�H����A���o�X�@�ӽШD, ��o�^��, �M��]�w`$scope.greeting.text`���󥦪�^����. Angular�|�۰ʧ��r��J�ةM���j�A������text���ӭ�.

###�̿�`�J

���e�ڭ̴���L, �b`HelloController`�����ܦh�F�賣�i�H����, �o�̧ڭ̨èS���s�g. �Ҧp, `$scope`�ﹳ�N�۰ʸj�w��ƨöǻ����ڭ�; �ڭ̤��ݭn�g�ѩI�s�����ƨӫإߥ�. �ڭ̥u�O�g�ѱN����m�bHelloController���c�y�����ӳX�ݥ�.

���p�ڭ̱N�b�᭱�����`���|�ݨ�, `$scope`�ä��O�ڭ̰ߤ@�i�H�X�ݪ��ƪ�. �p�G�ڭ̧Ʊ�N���ô����Τ��s������URL�a�}��, �ڭ̥i�H�g�ѱN�Ω�޲z������H`$location`��b�ڭ̪��c�y�����ӳX�ݥ�, �N���o��:
```js
    function HelloController($scope, $location){
        $scope.greeting = {text: 'Hello'};
        //use $location for something good here...
    }
```
�ڭ̸g��Angular���̿�`�J�t�ιF��o�ӯ��_���ĪG. �̿�`�J���ڭ̱o�H����o�ض}�o������, �Ӥ��ݭn�إߨ̿�, �ڭ̪����u�ݭn���D���ݭn����.

�b�����e, ���O�@�ӳQ�٬��o���֦թw�ߪ��]�p�Ҧ�, �q�`�]�Q�٧@�̤֪��ѭ�h. �ѩ�ڭ̪�HelloController���u�@�u�O�]�wgreeting�ҫ�����ժ��A, �o�ؼҦ��|�i�D�A�L�ݾ�ߨ�L���Ʊ�, �Ҧp`$scope`�O�p��إߪ�, �Ϊ̦b���̥i�H��쥦.

�o�ӯS�ʨä��u�O�g��Angular�ج[�إߪ���H�~��. �A�]�i�H��n�����ӳo�ӭ���s�g��L���N�X.

###���O

Angular�̦n���������@�N�O�A�i�H�p�P�s�gHTML�@�˽s�g�A���˪O. ���ҥH�i�H�o�˰�, �O�ѩ�o�Ӯج[���֤߳����ڭ̤w�g�]�t�F�@�Ӫ�DOM�ѪR����, �����\�A�X�RHTML���y�k.

�ڭ̤w�g�b�ڭ̪��˪O���ݨ�F�@�Ǥ��ݩ�HTML�W�d���ݩ�. �Ҧp�]�t�b�j�A���������ô��, �Ω���w���ӱ���������������Ϫ�`ng-controller`, �H�ε���J�ظj�w�@�Ӽҫ���`ng-model`. �o�ǧڭ̳�����HTML�X�R���O.

Angular�a���\�h���w, �H���U�A�w�q���ε{��������. �ܧ֧ڭ̴N�|�ݨ��h�����O. �o�ǫ��O�i�H�w�q�ӧڭ̳q�`�Χ@���Ϫ��˪O��. ���̥i�H�Ω��n���]�w�A�����ε{���p��u�@�Ϊ̫إߥi�_�Ϊ��ե�.

�A�ä��ȭ���ϥ�Angular�۱a�����O. �A�]�i�H�s�g�A�ۤv��HTML�˪O�X�R, ���A�Q�����Ʊ�. 

##�d��:�ʪ���

���ڭ̨Ӭݤ@�Ӹ��j���Ҥl, ���i�ܤF��h��Angular����O. �Q���@�U, �ڭ̭n�إߤ@���ʪ����ε{��. �b���ε{�����Y�Ӧa��, �ڭ̻ݭn�i�ܥΤ᪺�ʪ����ä��\�L�s��. ���U�ӧڭ̪������쨺����.
```html
    <html ng-app="myApp">
    <head>
    <title>Your Shopping Cart</title>
    </head>
    <body ng-controller="CartController">
        <h1>Your Order</h1>
        <div ng-repeat="item in items">
            <span{{item.title}}</span>
            <input ng-model="item.quantity" />
            <span>{{item.price | currency}}</span>
            <span>{{item.price * item.quantity | currency}}</span>
            <button ng-click="remove($index)">Remove</button>
        </div>
        <script src="angular.js"></script>
        <script>
        function CartController($scope){
            $scope.items = [
                {title: 'Paint pots', quantity: 8, price: 3.95},
                {title: 'Polka dots', quantity: 17, price: 12.95},
                {title: 'Pebbles', quantity: 5, price: 6.95}
            ];
            
            $scope.remove = function(index){
                $scope.items.splice(index, 1);
            }
        }
        </script>
    </body>
    </html>
```
��^���Τ�ɭ��I�̦p��1-4�ҥ�:

![shopping-cart](figure/shopping-cart.png)

��1-4 �ʪ����Τ�ɭ�

�U���O����o�ӽd�Ҫ�²�u�Ѧ�. ���Ѩ�l���������ѤF��`�J������.

���ڭ̱q�����}�l:
```html
    <html ng-app>
```
`ng-app`�ݩʧi�DAngular���Ӻ޲z���������@����. �ѩ�ڭ̧⥦��b`<html>`������, �o�N�i�DAngular�ڭ̧Ʊ楦�޲z��ӭ���. �o�����]�O�A�ҧƱ檺, ���O�p�G�A�O���X�{����Angular���ε{���ӨϥΨ�L�覡�޲z����, �A�i��Ʊ�⥦��b���ε{�������Y��`<div>`��.
```html
    <body ng-controller="CartController">
```
�bAngular��, �A�Ω�޲z�����ϰ쪺JavaScript���Q�٬����. �g�Ѧbbody���Ҥ��]�t�@�ӱ��, �ڭ��n���o��`CartController`�N�޲z`<body>`�M`</body>`�������Ҧ��ƪ�.
```html
    <div ng-repeat="item in items">
```
`ng-repeat`���N��N�O���Q�٬�`$items`���Ʋժ��C�@�Ӥ������ƻs�@��`<div>`����DOM. �b�C�@�ӽƻs��div�ƥ���, �ڭ̳��|����e�����]�w�@�ӦW��`item`���ݩ�, �]���ڭ̥i�H�b�˪O���ϥΥ�. ���p�A�Ҭݨ쪺, �o�N�ɭP�o�T��`<div>`���C�@�ӳ��]�t���~�����D, �ƶq, ���, �`���H�Τ@�ӥΩ󲾰���Ӷ������s.
```html
    <span>{{item.title}}</span>
```
���p�ڭ̦b"Hello, World"�Ҥl���ҥ�,  ���ô���g��`{{ }}`���ڭ̱N�ܼƪ��ȴ��J�쭶�������ëO���P�B. ���㪺��F��`{{item.title}}`�|���N�˯���eitem, �M��N��item�����D�ݩʲզ����e���J��DOM��.
```html
    <input ng-model="item.quantity">
```
��r��J�r�q�M`item.quantity`���Ȥ�����`ng-model`�w�q�ëإ߸��ô��.

`<span>`����`{{ }}`�Ω�]�w�@�ӳ�V���pô, �N��N�O"�b�o�̴��J�@�ӭ�". �o�O�ڭ̧Ʊ檺�ĪG, ���O��Τ���ܳ�������ε{���]�ݭn���D, �o�˥��N��������`��.

�ڭ̸g�Ѩϥ�`ng-model`�ӦP�B�ҫ������ܤ�. `ng-model`�n���N`item.quantity`���ȴ��J���r�줤, �C��Τ��J�@�ӷs���Ȯɥ��]����۰ʧ�s`item.quantity`����.
```html
    <span>{{item.price | currency}}</span>
    <span>{{item.price * item.quantity || currency}}</span>
```
�ڭ̧Ʊ����M�`���Q�榡�Ƭ������Φ�. Angular�۱a�F�@�Ӻ٬��L�o�����S�����ڭ̥i�H�ഫ��r, �o�̸j�w�F�@�Ӻ٬�`currency`���L�o���Ω󵹧ڭ̳B�z�o�̪������榡. �b�U�@���ڭ̱N�|�ݨ��h���L�o��.
```html
    <button ng-click="remove($index)">Remove</button>
```
�o���\�Τ�g���I�����~���䪺Remove���s�ӱq�L�̪��ʪ�������������. �ڭ̳]�w���I���o�ӫ��s�ɩI�s`remove()`���. �ڭ��ٵ����ǻ��F�@��`$index`, ���]�t�F`ng-repeat`���ޭ�, �]���ڭ̥i�H���D���@���N�|�Q����.
```js
    function CartController($scope)
```
�o��`CartContoller`�Ω�޲z�ʪ������޿�. �o�|�i�DAngular, ����ݭn�b�o�̵��L�]�w�@�Ӻ٬�`$scope`���F��. �o��$scope�Ω����ڭ̦b�Τ�ɭ����N���ô���줸����.
```js
    $scope.items = [
        {title: 'Paint pots', quantity: 8, price: 3.95},
        {title: 'Polka dots', quantity: 17, price: 12.95},
        {title: 'Pebbles', quantity: 5, price: 6.95}
    ];
```
�g�ѩw�q`$scope.items`, �ڭ̫إߤF�@�ӵ�������ƫ��ƪ�Ӵy�z�Τ��ʪ����������~��. �ڭ̧Ʊ楦�i�H�Ω�UI�������ô��, �]���N�L�K�[��$scope��.

��M, �@�ӯu�ꪩ�����ʪ������i��u�b���s���u�@, ���ݭn�X�ݦ��A�������T�s�x�����. �ڭ̱N�b�᭱�����`���Q�׳o��.
```js
    $scope.remove = function(index){
        $scope.items.splice(index, 1);
    }
```
�ڭ��٧Ʊ�`remove()`��Ư���Ω�Τ�ɭ��������ô��, �]���ڭ̦P�˱N���K�[��$scope��. ���o�Ӥu�@�b���s�����������ʪ���, `remove()`��ƥi�H�Y�ɱq�Ʋդ��R������. �ѩ�`<div>`�C��O�g��`ng-repeat`�إߪ����ô��, �ҥH���خ����ɦC��N�۰ʦ��Y. �O��, �C��Τ�bUI�W�I���@��Remove���s��, �o��`remove()`��ƴN�|�Q�I�s.

##�p��

�ڭ̤w�g�ݨ�FAngular�̰򥻪��Ϊk�H�Τ@�ǫD�`²�檺�Ҥl. ���ѫ᭱�������N�M�`�󤶲гo�Ӯج[���Ѫ��\��.
