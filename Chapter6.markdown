#���O

�����O, �A�i�H�X�RHTML�ӥH�K�[�n���ʻy�k�Ӱ�����A���w�����Ʊ�. �g�ѳo�˰�, �A�i�H�����@�ǯS�w��A�����ε{�����q�Ϊ�\<div\>s�M\<span\>s�����M�ݩʪ���ڷN�q. ���̳��a��Angular���Ѫ���¦�\��, ���O�A�i�H�إ߯S�w�����ε{�����A�ۤv�Q�����Ʊ�.

�����ڭ̭n�ƲߥH�U���OAPI�H�Υ��bAngular�ҰʩM�B��ͩR�g���̬O�p��B�@��. �q����, �ڭ̱N�ϥγo�ǥu�O�ӫإߤ@�ӫ��O����. �b���N�����ɧڭ̱N�ǲߨ�p��s�g���O���椸���թM�ϥ��̹B��o���.

���O����, �ڭ̨Ӭݬݤ@�ǨϥΫ��O���y�k����.

##���O�MHTML����

�b���Ѥ�, �ڭ̤w�g�ϥΤFAngular���m���O��`ng-directive-name`�y�k. �Ҧp`ng-repeat`, `ng-view`�M`ng-controller`. �o��, `ng`�����OAngular���R�W�Ŷ�, �åBdash���᪺�����K�O���O���W��.

���M�ڭ̳��w�o�Ӥ�K��J���y�k, ���O�b�j������HTML���Ҿ�������O���Ī�. ���F����o��, Angular���O���\�A�H�X�ؤ覡�I�s���N�����O. �H�U�b��6-1���C�X���y�k, ���O�������ï�����A���R��[���諸]���Ҿ����`�u�@

Table 6-1 HTML Validation Schemes

<table>
	<thead>
		<tr>
			<th>Validator</th>
			<th>Format</th>
			<th>Example</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>none</td>
			<td>namespace-name</td>
			<td>ng-repeat=<i>item in items</i></td>
		</tr>
		<tr>
			<td>XML</td>
			<td>namespace:name</td>
			<td>ng:repeat=<i>item in items</i></td>
		</tr>
		<tr>
			<td>HTML5</td>
			<td>data-namespace-name</td>
			<td>data-ng-repeat=<i>item in items</i></td>
		</tr>
		<tr>
			<td>xHTML</td>
			<td>x-namespace-name</td>
			<td>x-ng-repeat=<i>item in items</i></td>
		</tr>
	</tbody>
</table>

�ѩ�A�i�H�ϥΥ��N���o�ǧΦ�, [AngularJS���](http://docs.angularjs.org/)���C�X�F�@�Ӿm�p�������O, �Ӥ��O����o�ǿﶵ. �Ҧp, �b`ngRepeat`���D�U�A�i�H���`ng-repeat`. �y��A�|�ݨ�, �b�A�w�q�A�ۤv�����O�ɧA�N�|�ϥγo�ةR�W�榡.

�p�G�A���A��HTML���Ҿ�(�j�h�ƤH�����ϥ�), �A�i�H�ܦn���ϥΦb�ثe�A�Ҩ��L���Ҥl�����R�W�Ŷ�-���O[namespace-directive]�y�k

##API�w��

�U���O�@�ӫإߥ��N���O���N�X�˪O

	var myModule = angular.module(...);

	myModule.directive('namespaceDirectiveName', function factory(injectables) {
		var directiveDefinitionObject = {
			restrict: string,
			priority: number,
			template: string,
			templateUrl: string,
			replace: bool,
			transclude: bool,
			scope: bool or object,
			controller: function controllerConstructor($scope, $element, $attrs, $transclude){...},
			require: string,
			link: function postLink(scope, iElement, iAttrs) {...},
			compile: function compile(tElement, tAttrs, transclude){
				return: {
					pre: function preLink(scope, iElement, iAttrs, controller){...},
					post: function postLink(scope, iElement, iAttrs, controller){...}
				}
			}
		};
		return directiveDefinitionObject;
	});

���ǿﶵ�O���۱ƥ���, ���̤j�h�Ƴ��O�i�諸, �åB���̳��������Ȫ��Բӻ���:

��A�ϥΨC�ӿﶵ��, ��6-2���ѤF�@�ӷ��z.

Table 6-2 ���O�w�q�ﶵ

<table>
	<thead>
		<tr>
			<th>Property</th>
			<th>Purpose</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>restrict</td>
			<td>�n�����O�i�H�@���@�Ӥ���, �ݩ�, ��, �����Ϊ̥��N���զX�p��Ω�˪O��</td>
		</tr>
		<tr>
			<td>priority</td>
			<td>�]�w�˪O���۹���L�����W���O�����涶��</td>
		</tr>
		<tr>
			<td>template</td>
			<td>���O�@�ӧ@���r�Ŧꪺ���p�˪O. �p�G�A���w�@�Ӽ˪OURL�N���n�ϥγo�Ӽ˪O�ݩ�.</td>
		</tr>
		<tr>
			<td>templateUrl</td>
			<td>���w�g��URL�[�����˪O. �p�G�A���w�F�r�Ŧꪺ���p�˪O�N���ݭn�ϥγo��.</td>
		</tr>
		<tr>
			<td>replace</td>
			<td>�p�G��true, �h������e����. �p�G��false�Ϊ̥����w, �h�N�o�ӫ��O�l�[���e�����W.</td>
		</tr>
		<tr>
			<td>transclude</td>
			<td>���A�N�@�ӫ��O����l�۸`�I���ʨ�߼˪O��m��.</td>
		</tr>
		<tr>
			<td>scope</td>
			<td>���o�ӫ��O�إߤ@�ӷs���@�ΰ�Ӥ��O�~�Ӥ��@�ΰ�.</td>
		</tr>
		<tr>
			<td>controller</td>
			<td>������O�q�H�إߤ@�ӵo�G��API.</td>
		</tr>
		<tr>
			<td>require</td>
			<td>�ݭn��L���O�A�ȩ�o�ӫ��O�ӥ��T���o���@��.</td>
		</tr>
		<tr>
			<td>link</td>
			<td>�H�s�{���覡�קﲣ�ͪ�DOM�������, �K�[�ƥ��ť��, �]�w���ô��.</td>
		</tr>
		<tr>
			<td>compile</td>
			<td>�H�s�{���覡�ק�@�ӫ��O��DOM�˪O���ƥ��S��, �p�P�ϥ�`ng-repeat`��. �A���sĶ��Ƥ]�i�H��^�챵��ƨӭקﲣ�ͤ��������.</td>
		</tr>
	</tbody>
</table>

�U�����ڭ̲`�J�Ӹ`�Ӭݬ�.

###���A�����O�R�W

�A�i�H�μҲժ����O��Ƭ��A�����O�إߤ@�ӦW��, �p�U�ҥ�:

	myModule.directive('directiveName', function factory(injectables){...});

���M�A�i�H�ϥΥ���A���w���W�r�R�W�A�����O, �ӲŸ��|��ܤ@�ӫe��R�W�Ŷ����ѧA�����O, �P���קK�P�i��]�t�b�A�����ؤ����~�����O�Ĭ�.

�A��M���Ʊ楦�̨ϥΤ@��`ng-`�e��, �]���o�i��PAngular�۱a�����O�۽Ĭ�. �p�G�A�q�Ʃ�SuperDuper MegaCorp, �A�i�H��ܤ@��super-, superduper-, �Ϊ̬ƦܬOsuperduper-megacorp-, ���M�A�i���ܲĤ@�ӿﶵ, �u�O���F��K��J.

���p�e���Ҵy�z��, Angular�ϥΤ@�ӼзǤƪ����O�R�W����, �åB�չϦ��Ī��b�˪O���ϥξm�p�������O�R�W�覡�ӽT�O�b5�Ӥ��P���ͦn�����Ҿ������`�u�@. �Ҧp, �p�G�A�w�g��ܤF`super-`�@���A���e��, �åB�A�b�s�g�@�Ӥ�����(datepicker)�ե�, �A�i��N���R�W��`superDatePicker`. �b�˪O��, �A�i�H���o�˨ӨϥΥ�: `super-date-picker`, `super:date-picker`, `data-super-date-picker`�Ϊ̨�L�h�˪��Φ�.

###���O�w�q�ﹳ

���p�e�����쪺, �b���O�w�q���j�h�ƪ��ﶵ���O�i�諸. ��ڤW, �o�̨èS���w�ʪ��n�D������ܭ��ǿﶵ, �åB�A�i�H�c�y�X�\�h���Q����O���l���Ѽ�. ���ڭ̨ӳv�B�Q�׳o�ǿﶵ�O������.

####restrict

`restrict`�ݩʤ��\�A���w�A�����O�n������--�]�N�O��, ���O�_����Ω�@�������W��, �ݩ�, ��[className], �Ϊ̵���. �A�i�H�ھڪ�6-3�ӫ��w�@�өΦh���n������, �u�ݭn�ϥΤ@�Ӧr�Ŧ�Ӫ�ܨ䤤���C�@������:

Table 6-3 ���O�n���Ϊk�ﶵ

<table>
	<thead>
		<tr>
			<th>Character</th>
			<th>Declaration style</th>
			<th>Example</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>E</td>
			<td>element</td>
			<td>&lt;my-menu title=<i>Products</i>&gt;&lt;/my-menu&gt;</td>
		</tr>
		<tr>
			<td>A</td>
			<td>attribute</td>
			<td>&lt;div my-menu=<i>Products</i>&gt;&lt;/div&gt;</td>
		</tr>
		<tr>
			<td>C</td>
			<td>class</td>
			<td>&lt;div class=my-menu:<i>Products</i>&gt;&lt;/div&gt;</td>
		</tr>
		<tr>
			<td>M</td>
			<td>comment</td>
			<td>&lt;!--directive:my-menu Products--&gt;</td>
		</tr>
	</tbody>
</table>

�p�G�A�Ʊ�A�����O�Χ@�@�Ӥ����Ϊ̤@���ݩ�, ����A���Ӷǻ�`EA`�@��`restrict`�r�Ŧ�.

�p�G�A�����F`restrict`�ݩ�, �h�q�{��`A`, �åB�A�����O�u��Χ@�@���ݩ�(�ݩʫ��O).

�p�G�A�p�����IE8, ������attribute-�Mclass-�����O�N�O�A�̦n�����, �]�����ݭn�B�~���V�O�ӨϷs�������`�u�@. �i�H�d��Angular���ӸԲ��A�ѳo�@�I.

####Priorities

�b�A���h�ӫ��O�j�w�b�@�ӳ�W��DOM�����ín�T�w���̪����ζ��Ǫ����p�U, �A�i�H�ϥ�`priority`�ݩʨӫ��w���Ϊ�����. �ƭȰ��������B��. �p�G�A�S�����w, �h�q�{��priority��0.

�����o�ͻݭn�]�w�u���Ū����p. �@�ӻݭn�]�w�u���ŨҤl�O`ng-repeat`���O. ���Ƥ�����, �ڭ̧Ʊ�Angular�b���Ϋ��O���e�ɦb�@�Ӽ˪O�������ƥ�. �p�G���o��, ��L�����O�N�|���Ψ�зǪ��˪O�����W�Ӥ��O�ڭ̩ҧƱ�b���ε{�������Ƨڭ̪�����.

���M��(proority)���b���, ���O�A�i�H�j�MAngular�귽���ּƴX�Өϥ�`priority`����L���O. ���`ng-repeat`, �ڭ̨ϥ��u���ŭȬ�1000, �o�˴N���������u���ųB�z�u���B�z��.

####Templates

��إ߲ե�, ����, ����@�_��L�F���, Angular���\�A���Ѥ@�Ӽ˪O�����Ϊ̥]�q���������e. �Ҧp, �p�G�A�b���Ϥ��إߤ@��tab�ﶵ�d, �i��|�e�{�X�p��6-1�ҥܵ���.

![tab](figure/tab.png)

��6-1 tab�ﶵ�d����

�ä��O�@��\<div\>, \<ul\>\<li\>�M\<a\>����, �A�i�H�إߤ@��\<tab-set\>�M\<tab\>���O, �Ψ��n���C�ӳ�W��tab�ﶵ�d�����c. �M��A��HTML�i�H������n�Ӫ�F�A���˪O�N��. �̲׵��G�i��ݰ_�ӹ��o��:

	<tab-set>
		<tab title="Home">
			<p>Welcome home!</p>
		</tab>
		<tab title="Preferences">
			<!-- preferences UI goes here -->
		</tab>
	</tab-set>

�A�٥i�H��title�j�w�@�Ӧr�Ŧ���, �g�Ѧb\<tab\>�Ϊ�\<tab-set\>�W�j�w����B�ztab�ﶵ���e. �����ȭ���Φbtabs�W--�A�٥i�H�Ω���, �⭷�^, �u��, dialog��ܮةΪ̨�L����A�Ʊ�H�o�ؤ覡��{���a��.

�A�i�H�g��`template`�Ϊ�`templateUrl`�ݩʨӫ��w������DOM����. �ϥ�`template`�g�Ѧr�Ŧ�ӳ]�w�˪O���e, �Ϊ̨ϥ�`templateUrl`�ӱq���A�����@�Ӥ��W�ӥ[���˪O. ���p�A�b���U�Ӫ��Ҥl���|�ݨ�, �A�i�H�w���֨��o�Ǽ˪O�Ӵ��GET�ШD, �o���Q�󴣰����Ϊ��ʯ�.

���ڭ̨ӽs�g�@��dumb���O: �@��\<hello\>����, �u�O�Ω�ϥ�\<div\>Hi there\</div\>�Ӵ����ۨ�. �b�o��, �ڭ̱N�]�w`restrict`�Ӥ��\�����M�]�w`template`��ܧڭ̩ҧƱ檺�F��. �ѩ��q�{���欰�u�N���e�l�[�줸����, �]���ڭ̱N�]�w`replace`�ݩʬ�true�Ӵ�����Ӫ��˪O:

	var appModule = angular.module('app', []);
	appModule.directive('hello', function(){
		return {
			restrict: 'E',
			template: '<div>Hi there</div>',
			replace: true
		};
	});

�b�������ڭ̥i�H���o�˨ϥΥ�:

	<html lang="en" ng-app="app">
	...
	<body>
		<hello></hello>
	</body>
	...

�N�����J���s������, �ڭ̷|�ݨ�"Hi there".

�p�G�A�d�ݭ�������l�X, �b�����W�A���M�|�ݨ�\<hello\>\</hello\>, ���O�p�G�A�d�ݲ��ͪ���l�X(�bChrome��, �A�i�H�b"Hi there"�W�k���M���ܼf�d����), �A�|�ݨ�:

	<body>
		<div>Hi there</div>
	</body>

\<hello\>\</hello\>�Q�˪O����\<div\>�����F.

�p�G�A�q���O�w�q������`replace: true`, ����A�|�ݨ�\<hello\>\<div\>Hi there\</div\>\</hello\>.

�q�`�A�|�Ʊ�ϥ�`templateUrl`�Ӥ��O`template`, �]����JHTML�r�Ŧ�ä��O���򦳽�. `template`�ݩʳq�`���Q��D�`�p���˪O. �ϥ�templateUrl`�P�˫D�`����, �i�H�]�w�A���Y�Өϼ˪O�i�֨�. �ڭ̥i�H���U���o�˭��g�ڭ̪�`hello`���O:

	var appModule = angular.module('app', []);
	appModule.directive('hello', function(){
		return {
			restrict: 'E',
			templateUrl: 'helloTemplate.html',
			replace: true
		};
	});

�b`helloTemplate.html`��, �A�u�ݭn��J:

	<div>Hi there</div>

�p�G�A�ϥ�Chrome�s����, ����"�P������"�|��´Chrome�q`file://`���[���o�Ǽ˪O, �åB�A�|�o��@������"Origin null is not allowed by Access-Control-Allow-Origin."�����~. ����b�o��, �A����ӿ��:

+ �g�Ѧ��A���ӥ[������
+ �bChrome���]�w�@�Ӽлx. �A�i�H�g�Ѧb�R�O�椤�ϥ�`chrome --allow-file-access-from-files`�R�O�ӹB��Chrome����o�@�I.

�o�N�|�g��`templateUrl`�[���o�Ǥ��, �M��, �o�|���A���Τ�n���ݨ���O�[��. �p�G�A�Ʊ�b�����[���˪O, �A�i�H�b�@��`script`���Ҥ��N���@���o�ӭ������@�����]�t�i��, �N���o��:

	<script type="text/ng-template" id="helloTemplateInline.html">
		<div>Hi there</div>
	</script>

�o�̪�id�ݩʫܭ��n, �]���o�OAngular�ΨӦs�x�˪O��URL��. �y�ԧA�N�|�ϥγo��id�b���O��`templateUrl`�����w�n���J���˪O.

�o�Ӫ�������ܦn�����J�Ӥ��ݭn���A��, �]���S�����n��`XMLHttpRequest`�Ө��o���e.

�̫�, �A�i�H�V�L`$http`�Ϊ̥H��L����ӥ[���A�ۤv���˪O, �M��N���̪����]�w�bAngular���٬�`$templateCache`����H�W. �ڭ̧Ʊ�b���O�B�椧�e�֨������o�Ӽ˪O�i��, �]���ڭ̱N�g��module�W��run��ƨөI�s��.

	var appModule = angular.module('app', []);

	appModule.run(function($templateCache){
		$templateCache.put('helloTemplateCached.html', '<div>Hi there</div>');
	});

	appModule.directive('hello', function(){
		return {
			restrict: 'E',
			templateUrl: 'helloTemplateCached.html',
			replace: true;
		};
	});

�A�i��Ʊ�b���~���o��, �ȶȧ@���@�Ӵ�֩һݪ�GET�ШD�ƶq���޳N. �A�i�H�B��@�Ӹ}���N�Ҧ����˪O�X�֨�@�ӳ�W�����, �æb�@�ӷs���Ҳդ��[����, �M��A�N�i�H�q�A���D���ε{���Ҳդ��ޥΥ�.

####Transclusion

���F�����Ϊ̰l�[���e, �A�٥i�H�g��`transclude`�ݩʱN��Ӫ����e����s�˪O��. ��]�w��true��, ���O�N�R����Ӫ����e, ���O�b�A���˪O���g�Ѥ@�ӦW��`ng-transclude`�����O���s���J�Өϥ��i��. 

�ڭ̥i�H�ϥ�transclusion�ӧ��ܧڭ̪��d��:

	appModule.directive('hello', function() {
		return {
			template: '<div>Hi there <span ng-transclude></span></div>',
			transclude: true
		};
	});

���o�˨����Υ�:

	<div hello>Bob</div>

�A�|�ݨ�: "Hi there Bob."

###�sĶ�M�챵�\��

���M���J�˪O�O���Ϊ�, ������O�u�����쪺�u�@�o�ͦb����`compile`�M����`link`��Ƥ�.

`compile`�M`link`��ƳQ���w��Angular�Ψӫإ����ε{����ڵ��Ϫ����Ӷ��q. ���ڭ̱q�󰪼h���Ӭݬ�Angular����l�ƹL�{, ���@�w������:

**Script loads**

Angular�[���M�d��`ng-app`���O�ӧP�w���ε{���ɭ�.

**Compile phase(���q)**

�b�o�Ӷ��q, Angular�|�M��DOM�`�I�H�T�w�Ҧ����U�b�˪O�������O. ���C�@�ӫ��O, �M������O���W�h(`template`,`replace`,`transclude`����)�ഫDOM, �åB�p�G���s�b�N�I�s`compile`���. ������^���G�O�@�ӽsĶ�L��`template`���, �o�N�q�Ҧ������O���I�s`link`��ƨӦ���.

**Link phase(���q)**

�إ߰ʺA������, �M��Angular�|��C�ӫ��O�B��@��`link`���. `link`��Ƴq�`�bDOM�Ϊ̼ҫ��W�إߺ�ť��. �o�Ǻ�ť���Ω���ϩM�ҫ��b�Ҧ����ɶ��̳��O���P�B.

�]���ڭ̥����b�sĶ���q�B�z�˪O���ഫ, �P�ɦb�챵���q�B�z�b���Ϥ��ק���. ���ӳo�ӫ��, ���O����`compile`�M`link`��Ƥ����D�n���ϧO�O`compile`��ƳB�z�˪O�ۨ����ഫ, ��`link`��ƳB�z�b�ҫ��M���Ϥ����гy�@�ӰʺA���s��. �@�ΰ챾����sĶ�L��`link`��ƥ��O�b�o�ӲĤG���q, �åB�g�Ѹ��ô���N���O�ܦ����ʪ�.

�X��ʯ઺�Ҽ{, �̨�Ӷ��q�~���}��. `compile`��ƶȦb�sĶ���q����@��, ��`link`��Ʒ|�Q����h��, ��C�ӫ��O���. �Ҧp, ���ڭ̨ӻ����A�W���ϥΪ�`ng-repeat`���O. �A�ä��Q�p�i`compile`, �o�^�ɭP�b�C��`ng-repeat`���Ʈɳ����ͤ@��DOM�M�����ާ@. �ۤ�, �A�|�Ʊ�@���sĶ, �M���챵.

���M�A�@�L�ðݪ����Ӿǲ߽sĶ�M�챵���������P, �H�ΨC�ӥ\��, �A�ݭn�s�g���j���������O�����ݭn�ഫ�˪O; �A�ٷ|�s�g�j�������챵���.

���ڭ̦A�ݬݨC�ӻy�k�Ӥ���@�U, �ڭ̦�:

	compile: function compile(tElement, tAttrs, transclude) {
		return {
			pre: function preLink(scope, iElement, iAttrs, controller) {...},
			post: function postLink(scope, iElement, iAttrs, controller) {...}
		}
	}

�H���챵:

	link: function postLink(scope, iElement, iAttrs) {...}

�`�N�o�̦��@�I���P���O`link`�����o�F�@�ӧ@�ΰ쪺�X��, ��`compile`�S��. �o�O�]���b�sĶ���q����, �@�ΰ�ä��s�b. �M�ӧA����O�q`compile`��ƪ�^`link`���. �o��`link`��Ư���X�ݨ�@�ΰ�.

�٭n�`�N���O`compile`�M`link`���|��o�@�Ө쥦�̹�����DOM�K�N�M�o�Ǥ����ݩ�[attributes]�C���ޥ�. �o�̪��@�I�ϧO�O`compile`��ƬO�q�˪O����o�˪O�����M�ݩ�, �åB�|���o��`t`�e��. ��`link`��ƨϥμ˪O�إߪ����Ϲ�Ҥ���o���̪�, ���̷|���o��`i`�e��.

�o�ذϧO�u�s�b�����O����L���O���s�y�˪O�ƥ����ɭ�. `ng-repeat`�N�O�@�ӫܦn���Ҥl.

	<div ng-repeat="thing in things">
		<my-widget config="thing"></my-widget>
	</div>

�o��, `compile`��ƱN�u�Q�I�s�@��, ��`link`��Ʀb�C���ƻs`my-widget`�ɳ��|�Q�I�s�@��--�����󤸯��bthings�����ƶq. �]��, �p�G`my-widget`�ݭn��Ҧ�`my-widget`�ƥ�(���)���ק�@�Ǥ��@���F��, ���F���ɮĲv, ���T�����k�O�b`compile`��Ƥ��B�z. 

�A�i���ٷ|�`�N��`compile`��Ʀn�@���F�@��`transclude`�ݩʨ��. �o��, �A�٦����|�H�s�g�@�Ө�ƥH�s�{���覡transcludes���e, ���²�檺�����˪O�����Htransclusion�����p.

�̫�, `compile`�i�H��^�@��`preLink`�M`postLink`���, ��`link`�ȶȫ��V�@��`posyLink`���. `preLink`, ���p�����W�r�ҷt�ܪ�, ���B��b�sĶ���q����, ���O�|�b���O�챵��l�������e. �P�˪�, `postLink`�|�B��b�Ҧ����l�������O�Q�챵����. �o�N���ۦp�G�A�ݭn����DOM���c, �A�N�b`posyLink`���B�z. �b`preLink`���B�z�N�|�V�c�y�{�þɭP�@�ӿ��~.

###�@�ΰ�

�A�|�g�`�Ʊ�q���O���X�ݧ@�ΰ�Ӻʱ��ҫ����Ȩæb���̧��ܮɧ�sUI, �P�ɦb�~���ɶ��y���ҫ����ܮɳq��Angular. �̮ɳ̱`����, ��A�qjQuery, Closure�Ϊ̨�L�w���]�q�@�ǫDAngular�ե�Ϊ̹�{²�檺DOM�ƥ��. �M��NAngular��F���@���ݩʶǻ���A�����O���Ӱ���. 

�o�]�O�A����ϥΤ@�ӧ@�ΰ쪺��]���@, �A�i�H��o�T���������@�ΰ�ﶵ:

1. �q���O��DOM��������o**�{�����@�ΰ�**.
2. �إߤ@��**�s�@�ΰ�**, ���~�ӦۧA���X������@�ΰ�. �o��, �A���L����X�ݾ�W�h�@�ΰ줤���Ҧ���. �o�ӧ@�ΰ�N�|�ШD�o�ا@�ΰ�P�ADOM��������L���N���O�@�ɥ��óQ�Ω�P���̳q�H.
3. �q�������h**�j���X�Ӫ��@�ΰ�**���a���ҫ��ݩ�. ��A�b�إߥi���Ϊ��ե�ӻݭn�q���@�ΰ줤�j�����O�ާ@��, �A�N�|�Ʊ�ϥγo�ӿﶵ.

�A�i�H�ϥΤU�����y�k�ӫإ߳o�ǧ@�ΰ��������t�m:

<table>
	<thead>
		<tr>
			<th>Scope Type</th>
			<th>Syntax</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>existing scope</td>
			<td>scope: false(�p�G�����w�N�ϥγo���q�{��)
		</tr>
		<tr>
			<td>new scope</td>
			<td>scope: true</td>
		</tr>
		<tr>
			<td>isolate scope</td>
			<td>scope: { /* attribute names and binding style */ }</td>
		</tr>
	<tbody>
</table>

��A�إߤ@�ӹj�����@�ΰ��, �q�{���p�U�A���ݭn�X�ݤ��@�ΰ줤�ҫ���������F��. �M��, �A�]�i�H���w�A�Q�n���S�w�ݩʶǻ���A�����O��. �A�i�H�{���O�a�o���ݩʦW�@���Ѽƶǻ�����ƪ�.

�`�N, ���M�j�����@�ΰ줣�N���ҫ��ݩ�, �����̤��M�O��Ƨ@�ΰ쪺����. �N���Ҧ���L�@�ΰ�@��, ���̳����@��`$parent`�ݩʤޥΨ쥦�̪�����.

�A�i�H�g�Ѷǻ��@�ӫ��O�ݩʦW���M�g���覡�q���@�ΰ�ǻ��S�w���ݩʨ�j�����@�ΰ줤. �o�̦��T�ئX�A���覡�q���@�ΰ줤�ǻ����. �ڭ̺ٳo�Ƕǻ���Ƥ��P���覡��"�j�w����". �A�]�i�H�i�諸���w�@�Ӱϰ�O�W���ݩʦW��.

�H�U�O�S���O�W���y�k:

	scope: {
		attributeName1: 'BINDING_STRATEGY',
		attributeName2: 'BINDING_STRATEGY',...
	}

�H�U�O�ϥΧO�W���覡:

	scope: {
		attributeAlias: 'BINDING_STRATEGY' + 'templateAttributeName',...
	}

�j�w�����Q�w�q����6-4�����Ÿ�:

��6-4 �j�w����

<table>
	<thead>
		<tr>
			<th>Symbol</th>
			<td>Meaning</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>@</td>
			<td>�N�ݩʧ@���r�Ŧ�ǻ�. �A�]�i�H�g�Ѧb�ݩʭȤ��ϥδ��ȲŸ�{{}}�ӱq���X���@�ΰ줤�j�w��ƭ�.</td>
		</tr>
		<tr>
			<td>=</td>
			<td>�ϥΧA�����O���Ƨ@�ΰ줤���@���ݩʸj�w��ƨ��ݩʤ�.</td>
		</tr>
		<tr>
			<td>&</td>
			<td>�q���@�ΰ줤�ǻ���@�Ө�Ƥ�, �H��I�s.</td>
		</tr>
	</tbody>
</table>

�o�ǳ��O�۷�⹳������, �]�����ڭ̨Ӭݤ@�Ө��骺�Ҥl�W���ܤƨӶi�满��. ��軡�ڭ̧Ʊ�إߤ@��`expander`���O�b���D��Q�I��������B�~�����e.

���Y�ɥ��ݰ_�Ӧp��6-2�ҥ�.

![6-2](figure/6-2.png)

��6-2 Expander in closed state

�i�}�ɥ��ݰ_�Ӧp��6-3�ҥ�.

![6-3](figure/6-3.png)

��6-3 Expander in open state

�ڭ̷|�s�g�p�U�N�X:

	<div ng-controller="SomeController">
		<expander class="expander" expander-title="title">
			{{text}}
		</expander>
	</div>

���D(Cliked me to expand)�M��r(Hi there folks...)���ȨӦ۩󳬦X���@�ΰ줤. �ڭ̥i�H���U���o�˨ӳ]�w�@�ӱ��:

	function SomeController($scope) {
		$scope.title = 'Clicked me to expand';
		$scope.text = 'Hi there folks, I am the content that was hidden but is now shown.';
	}

�M��ڭ̥i�H�ӽs�g���O:

	angular.module('expanderModule', [])
		.directive('expander', function(){
			return {
				restrict: 'EA',
				replace: true,
				transclude: true,
				scope: { title: '=expanderTitle'},
				template: '<div>' +
						'<div class="title" ng-click="toggle()">{{title}}</div>' +
						'<div class="body" ng-show="showMe" ng-tansclude></div>' +
						'</div>',
				link: function(scope, element, attris){
					scope.showMe = false;
					scope.toggle = function toggle(){
						scope.showMe = !scope.showMe;
					}
				}
			}
		});

�M��s�g�U�����˦�:

	.expander {
		border: 1px solid black;
		width: 250px;
	}
	.expander > .title {
		background-colo: black;
		color: white;
		padding: .1em .3em;
		cursor: pointer;
	}
	.expander > .body {
		padding: .1em .3em;
	}

���U�����ڭ̨Ӭݬݫ��O�����C�ӿﶵ�O������, �b��6-5��.

��6-5 Functions of elements

<table>
	<thead>
		<tr>
			<th>FunctionName</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>restrict: EA</td>
			<td>�@�Ӥ����Ϊ��ݩʳ��i�H�I�s�o�ӫ��O. �]�N�O��, \<expander ...\>...\</expander\>�P\<div expander...\>...\</div\>�O����</td>
		</tr>
		<tr>
			<td>replace:true</td>
			<td>�ϥΧڭ̴��Ѫ��˪O������l����</td>
		</tr>
		<tr>
			<td>transclude:true</td>
			<td>�N��l���������e���ʨ�ڭ̩Ҵ��Ѫ��˪O���t�~�@�Ӧ�m.</td>
		</tr>
		<tr>
			<td>scope: {title: =expanderTitle}</td>
			<td>�إߤ@�Ӻ٬�`title`���ϰ�@�ΰ�, �N���@�ΰ쪺�ݩʸ��ô�����n����`expanderTitle`�ݩʤ�. �o��, �ڭ̭��R�Wtitle�����K��expanderTitle. �ڭ̥i�H�s�g`scope: { expanderTitle: '='}`, ����b�˪O���ڭ̴N�n�ϥ�`expanderTitle`�F. ���O�b��L���O�]���@��`title`�ݩʪ����p�U, �bAPI������title���[�q�M�u�O���R�W���Ω�b�ϰ�ϥάO���N�q��. �Ъ`�N, �o�̦۩w�q���O�]�ϥΤF�ۦP���m�p���R�W�覡�@�����O�W.</td>
		</tr>
		<tr>
			<td>template: \<'div'\>+</td>
			<td>�n���o�ӫ��O�n���J���˪O. �`�N�ڭ̨ϥΤF`ng-click`�M`ng-show`����ܩM���æۨ��èϥ�`ng-transclude`�n���F��l���e�|�h����. �٭n�`�N���Otranscluded�����e����X�ݤ��@�ΰ�, �Ӥ��O���O���X�����@�ΰ�.</td>
		</tr>
		<tr>
			<td>link...</td>
			<td>�]�w`showMe`�ҫ����˴�expander���i�}/�������A, �P�ɩw�q�b�Ω��I��`title`�o��div���ɭԩI�s�w�q��`toggle()`���.</td>
		</tr>
	</tbody>
</table>

�p�G�ڭ̹��ϥΧ�h���N�q���F��Ӧb�˪O���w�q`expander title`�Ӥ��O�b�ҫ���, �ڭ��٥i�H�ϥζǻ��g�Ѧb�@�ΰ��n�����ϥ�`@`�Ÿ��ǻ��@�Ӧr�Ŧꭷ�檺�ݩ�, �N���U���o��:

	scope: { title: '@expanderTitle'},

�b�˪O���ڭ̴N�i�H��{�ۦP���ĪG:

	<expander class="expander" expander-title="Click mr to expand">
		{{text}}
	</expander>

�`�N, ���@�����ڭ̤��M�i�H�g�Ѩϥδ��J�k�Ntitle���ô����ڭ̪�����@�ΰ줤:

	<expander class="expander" expander-title="{{title}}">
		{{text}}
	</expander>

###�ާ@DOM����