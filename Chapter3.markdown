#�ĤT�� AngularJS�}�o

�{�b, �ڭ̤w�g���s�F�զ�AngularJS���@�ǽ��l. �ڭ̤w�g���D�Τ�i�J�ڭ̪����ε{����p����o���, �p����ܤ�r, �H�Φp�󰵤@�Ǯɻ쪺����, �L�o�M����DOM. ���O�ڭ̭n�p��⥦�̲�´�b�@�_�O?

�b����, �ڭ̱N�Q�ץH�U���e:

+ �p��A���ֳt�}�o���pAngularJS���ε{��
+ �Ұʦ��A���d�����ε{���欰
+ �ϥ�Karma�s�g�M�B��椸���թM��������
+ �w�ﲣ�~���p�sĶ�M���Y�A��AngularJS���ε{��
+ �ϥ�Batarang�����A��AngularJS���ε{��
+ ²�ƶ}�o�y�{(�q�إߤ���B�����ε{���M����)
+ �ϥΨ̿�޲z�wRequireJS��XAnguarJS����

�������b���Ѥ@��20000�^�ت����ϥH�i�D�A�p��i�檺���p�A��AngularJS���ε{��. �ڭ̤��|�i�J������ε{������. �b��4��, �`�J�@�ӨϥΩM�i�ܤF�U�ئU��AngularJS�S�ʪ��d�Ҥ@�ε{��.

##�M�׬[�c

���˨ϥ�Yeoman�c�اA������, �N�|���A��AngularJS���ε{���إߩҦ����n�����U�{�Ǥ��.

Yeoman�O�@�ӥ]�t�h�Ӯج[�M�Ȥ�ݮw���j�j���u��. ���g�Ѧ۰ʤƤ@�Ǥ�`���Ȫ��޾ɪ��覡���ѤF�@�ӧֳt���}�o���ҩM�W�j�A�����ε{��. �����ڭ̷|�ϥΤ@�ӧ��㪺�p�`���Цp��w�˩M�ϥ�Yeoman, ���O�b�����e, �ڭ̥���²�檺���ХH�U�ϥ�Yeoman�R�O���N���Ǥ�ʰ��檺�ާ@.

�ڭ��ٸԲӤ��ФF�A�Ψ����A�M�w���ϥ�Yeoman�����p, �]���bWindows���x���p����WYeoman�T��s�b�@�ǰ��D, �åB�]�w���ٵy�L���@�I�D�ԩ�.

��󨺨Ǥ��ϥ�Yeoman�����p, �ڭ̱N�|�ݬݤ@�ӽd�����ε{�����c(�i�H�bGithub�d�ҭܮw��`chapter3/sample-app`�ؿ������ - [�챵](https://github.com/shyamseshadri/angularjs-book/tree/master/chapter3/sample-app)), �U���O���˪����c, �]�O�ϥ�Yeoman���ͪ����c. ���ε{�������i�H�����H�U���O:

**JS��l�X**

�ݬ�`app/scripts`�ؿ�. �o�̬O�A�Ҧ���JS��l�X�Ҧb�ؿ�. �@�ӥD���ӵ��A�����ε{���]�wAngular�ҲթM����.

���~, �o���٦��@�ӳ�W�����--`app/scripts/controller`--�o�̭��O�U�ӱ��. ������Ѧ欰�M�o�G��ƨ�@�ΰ줤, �M����ܦb���Ϥ�. �q�`, ���̻P���ϳ��O�@�@������.

���O, �L�o���M�A�Ȥ]�i�H�b`app/scripts`�U�����, ���ެO�_�u���M����, �@���@�ӧ��㪺���(direcyives.js, filters.js, services.js)�Ϊ̳�Ӫ�����.

**Angular HTML�˪O���**

�{�b, �ϥ�Yeoman�إߪ��C�@��AngularJS�ϰ�˪O���i�H�b`app/views`�ؿ������. �o�O�M�g��j�h��`app/scripts/controller`�ؿ���.

�٦��t�~�@�ӭ��n��Angular�˪O���, �N�O�D�n��`app/index.html`. �o�Τ���oAngularJS��l�X, �]�O�A�����ε{���إߪ����N��l�X.

�p�G�A�̲׷|�إߤ@�ӷs��JS���, �n�T�O�⥦�K�[��`index.html`��, �P���٭n��s���D�ҲթM����(Yeoman�]�|���A���o��).

**JS�w�̿�**

Yeoman�b`app/scripts/vendor`�����A���ѤF�Ҧ���JS��l�X�̿�. �Q�b���ε{�����ϥ�[Underscore](http://underscorejs.org/)�M[SocketIO](http://socket.io/)? �S���D--�N�̿�K�[��vendor�ؿ���(�٦��A��`index.html`), �ö}�l�b�A���Υε{�Ǥ��ޥΥ�.

**�R�A�귽**

�̲קA�إߤF�@��HTML���ε{��, ���ٷ|�Ҽ{��A�����ε{���٦��@���ݭn��CSS�M�Ϲ��̿�. `app/styles`�M`app/img`�ؿ��N�O�X��o�ӥت��Ӳ��ͪ�. �A�u�ݭn�K�[�A�ݭn���F���ؿ����æb�A�����ε{�����ޥΥ���(��M, �n�ϥΥ��T��������|).

> �q�{���p�UYeoman���|�إ�`app/img`���|.

**�椸����**

���լO�D�`���n��, �åB���A�Ψ�AngularJS�ɬO�@���O�O��. �b���դ譱`test/spec`�ؿ����ӬM�g��A��`app/scripts`�ؿ�. �C�Ӥ�����Ӧ��@�ӥ]�t�����椸���ժ�spec���M�g(�蹳). �ؤl���|���C�ӱ�����إߤ@�Ӧs�ڤ��, �b`test/spec/controllers`�ؿ��U, �P��Ӫ�����㦳�ۦP���W��. ���̳��OJasmine���檺�W�d, �y�z�F�C�ӱ���w���欰���W�d.

**��X����**

AngularJS�۱a�F�ݹ�ݪ����դ���H���T���覡���m��w�̭�. �A�Ҧ���Jasmine�W�d�Φ���E2E(�ݹ��)����, ���O�s�b`tests/e2e`�ؿ��U.

> �q�{���p�UYeoman���|�إ�`test/�ؿ�`.

> ���ME2E���եi��ݰ_�ӹ�Jasmine, ����ڤW���O��. ���̪���ƬO�D�P�B���檺, �ӥ���, �i�H�g��Angular�����B�澹(Angular Scenario Runner)�B��. �]�����n�����������`���p�UJasmine���թҰ����Ʊ�(���ϥ�console.log���ƿ�X�@�ӭȪ����p).

�ٲ��ͤF�@��²�檺HTML���, �i�H�b�s���������}���Ӥ�ʪ��B�����. �M��Yeoman���|���ͦs�ڤ��, ���O���̿�`�ۦ����檺�椸����.

**�t�m���**

�o�̻ݭn��Ӱt�m���. �Ĥ@�ӬO`karma.conf.js`, �o�OYeoman���A���ͪ��Ω�B��椸���ժ�. �ĤG��, �OYeoman���|���ͪ�`karma.e2e.conf.js`. �o�Ω�B���������. �b�����������~��RequireJS�@�`�����@��²�檺���. �o�Ω�t�m�̿����Y���Ա�, �P�ɳo�Ӥ��Φb�A�ϥ�karma�B��椸���ժ��ɭ�.

�A�i��|��: �p��B��ڪ����ε{��? ����O�椸����? �ƦܧڸӦp��s�g�A�̩ҰQ�ת��o�ئU�˪��s��?

�O���, �~�����K�g, �Ҧ����o�Ǧb�A���ɶ����|����. �b�o�@���̭�, �ڭ̱N�B�z�]�w���ةM�}�o���Ҫ����D, �]���@���ڭ̺U�J�@����H���N�X, ���ǰ��D���i�H�ֳt���a�L. �A�ҽs�g���N�X�H�Φp��N���̻P�A�̲ת���H�����ε{���pô�b�@�_�����D, �ڭ̱N�b���U�Ӫ��X�����Q��.

##�u��

AngularJS�u�O�A�}�o��ں������u��c���@����. �b�o�@�`, �ڭ̱N�@�_�}�ݬݤ@�ǧA�ΥH�T�O���ĩM�ֳt�}�o�����P���u��, �qIDEs����չB�澹�찻���u��.

###IDEs

���ڭ̱q�A�p��s�g��l�X�}�l. ���j�q��JavaScript�s�边�i�H���, ���K�O���]���I�O��. ���ɶ��H�Ӫ��ƹ��ҩ�Emacs�MVi�O�}�oJS���̦n���. �{�b, �U��IDEs���۱a�F�y�k���G, �۰ʧ����H�Ψ�L�\��, �����A�@�ӿ�ܪ��l�a, �o�i��O�ȱo��. ����, ���ӨϥΨ��@�өO?

�p�G�A�����N�I�X�Q����(���ޥ����@��30�Ѫ��K�O�եδ�), [WebStorm](www.jetbrains.com/webstorm/��)�O�Ӥ��������, ���ɥN, WebStorm��JetBrains���ѤF�̼s�x��Web�}�o���x. ���Ҩ㦳���S��, �b���e�u���j�����y���~��, �]�A�N�X�۰ʧ���(�p��3-1�ҥ�, ���w�s��������), �N�X�ɯ�, �y�k�M�h�L���G, �P�ɤ���h�Ө禡�w�M�ج[���ҰʧY�i�ϥ�. ���~, ���ٺ}�G����X�F�bIED�����T������JavaScript���\��, �ӥB�o�ǳ��O���Chrome���檺.

![ide](figure/3-1.png)

�̤j���A���ӦҼ{�ϥ�WebStorm�}�oAngularJS��]�O���O�ߤ@�~��AngularJS����IDEs. �o�Ӵ������b�A��HTML�˪O�����T���۰ʧ���AngularJS��HTML����. �o�ǳ��O�`�Ϊ��N�X���q, �_�h�A�C�����n��J���ꪺ�N�X���q. �]�������ӹ��U���o�˿�J:

	directive('$directiveName$', function factory($injectables$){
		var directiveDefinitionObject = {
			$directiveAttr$;
			compile: function complie(tElement, tAttrs, transclude){
				$END$;
				return function(scope, elements, attrs){
					//...
				}
			}
		};
		return directiveDefinitionObject;
	});

�bWebStorm��, �A�i�H�u��J�H�U���e:

	ngdc

�M���`Tab`����o�P�˪��N�X. �o�u�O�j�h�ƥN�X�۰ʧ������󴣨Ѫ��\�ध�@.

##�B��A�����ε{��

�{�b���ڭ̰Q�צp��B��Ҧ��A�Ұ����Ʊ� - �d�����ε{�����ʰ_��, �b�s������. �u�ꪺ�P���H�U���ε{���O�p��u�@, �ڭ̻ݭn�@�Ӧ��A���ӪA�ȩ�ڭ̪�HTML�MJavaScript�N�X. �ڱN���Q��ؤ覡, �@�ثD�`²�檺�覡�O�ϥ�Yeoman�B�����ε{��, �t�~�@�ؤ��O�ܮe��������Yeoman����k, ���O�P�˫ܦn.

###�ϥ�Yeoman

Yeoman���A��²�檺�ϥΤ@��Web���A���A�ȧA�Ҧ����R�A�귽�M������JavaScript���. �u�ݭn�B��H�U�R�O:
	
	yeoman server

���N�Ұʤ@�Ӧ��A���P�ɦb�A���s���������}AngularJS���ε{�����D��. �C��A���ܧA����l�X��, ���Ʀܷ|��s(�۰ʨ�s)�s����. �ܻŤ��O��?

###���ϥ�Yeoman

�p�G���ϥ�Yeoman, �A�i��ݭn�t�m�@�Ӧ��A���ӪA�ȧA�Ҧ��D�ؿ��������. �p�G�A�����D�@��²�檺��k����o�@�I, �Ϊ̤��Q���O�ɶ��إߧA�ۤv��Web���A��, �A�i�H�bNode.js���ϥ�ExpressJS�ֳt���s�g�@��²�檺Web���A��(�u�n²�檺�ϥ�`npm install -g express`�Ө��o��). ���i��ݰ_�ӹ��U���o��:

	//available at chapter3/sample-app/web-server.js

	var express = require('express'),
	    app = express(),
	    port = parseInt(process.env.PORT, 10) || 8080;
		app.configure(function(){
			app.use(express.methodOverride());
			app.use(express.bodyParser());
			app.use(express.static(__dirname + '/'));
			app.use(app.router);
		});

	app.listen(port);
	console.log("Now serving the app at http://localhost:" + port + "app");

�@���A���F�o�Ӥ��, �A�N�i�H�ϥ�Node�B��o�Ӥ��, �g�ѨϥΤU�����R�O:

	node web-server.js

�P�ɥ��N�b8080�ݤf�Ұʦ��A��(�Ϊ̧A�ۤv��ܺݤf).

�i�諸, �b���ε{����󧨤��ϥ�Python�A���ӹB��:

	python -m SimpleHTTPServer

�L�קA�O�_�M�w�~��, �@���A�t�m�n���A���ùB��_��, ���N�Q�ɯ�ɤU����URL:

	http://localhost:[port-number]/app/index.html

�M��A�N�i�H�b�s�������d�ݧA���إߪ����ε{��. �`�N, �A�ݭn��ʪ���s�s�����Ӭd�ݧ���, ���P��ϥ�Yeoman.

##����AngularJS

���e�w�g���L(�Ʀܦb�������e��), �ڭ̦A���s���@��: ���լO�����i�֪�, AngularJS�Ͻs�g�X�z���椸���թM��X�����ܱo��²��. ���MAngularJS�ϥΦh�Ӵ��չB�澹�B�檺�ܦn, ���ڭ̰�H[Karma](http://karma-runner.github.io/0.8/index.html)�ӹL�j�h�ƧA�һݭn�����ѱj�j, ���M�Ψ�ֳt���B�澹.

###Karma

Karma�s�b���D�n����]�O�����A�������X�ʶ}�o(TDD)�y�{�ܱo²��, �ֳt�M����. ���ϥ�NodeJS�MSocketIO(�A���ݭn���D���̬O����, �u�ݭn���]���̬O�ܴΫܻŪ��禡�w), �ä��\�b�h���s�������Ψ�ֳt���B��A���N�X�M����. �b[https:// github.com/vojtajina/karma/](https:// github.com/vojtajina/karma/)���i�H����h�T��.

> **TDD²��**
>
> �����X�ʶ}�o�Ϊ�TDD, �O�@�Ӹg�ѽT�O�b�}�o�ͩR�g���������s�g���ժ��ӱ���k, �o�O�b�N�X��{���e�i�檺, �o�N�O�����X�ʪ��}�o(���u�O�@���@�����Ҥu��).
>
> TDD����h��²��:
> 
+ �N�X�u�ݭn�b�@�өһݭn���N�X���ե��Ѯɽs�g.
+  �s�g�̤֪��N�X�H�T�O���ոg��.
+  �b�C�@�B�R�����ƥN�X.
+  �@���Ҧ������ոg��, ���U�ӴN�O���U�@�өһݭn���\��K�[���Ѵ���.
>
> �H�U�O�T�O�o�ǭ�h��²��W�h:
>
+ ����´���}�o�A���N�X, �C�@��N�X���n���ت����s�g.
+ �A���N�X���M�O���׼Ҳդ�, ��K���X�M�i�_�Ϊ�(�A�ݭn������ե�)
+ ���Ѥ@�t�C�����������զC��, �H��������}�a�MBugs.
+ ���դ]���ӥR��W�d�M���, �H�A������ݭn�M�ܤ�.
>
> �bAngularJS���ڭ̵o�{�o�O�u��, �P�ɦb���AngularJS�N�X�w���ڭ̳��O�ϥ�TDD�Ӷ}�o. ���JavaScript�o�˪��L�ݽsĶ���ʺA�y��, �ڭ̰�H�}�n���椸���եi�H����Ӫ��Y�h.

����, �ڭ̦p����o�g�H��Karma�O? �n�a, �����T�O�b�A�������W�w�ˤFNodeJS. ���۱a�FNPM(Node�]�޲z��), �o�ϱo������޲z�M�w�˦��d�W�U��NodeJS�i�Ϊ��禡�w.

�@���A�w�ˤFNodeJS�MNPM, �w��Karma�u�ݭn²�檺�B��U�����R�O:

	sudo npm install -g karma

��o��. �A�u�n²�檺�T���Ӷ}�l�ϥ�Karma(�ڭ�~���F, �Ф��n�A�ѥ��{��W�O���ϥΪ�).

**���o�t�m���**:

�p�G�A�O��Yeoman�إ����ε{�����[, ����A�N�w�g���@�Ӳ{����Karma�t�m��󵥧A�Өϥ�. �p�G���O, �����~��, �åB�b�A�����ε{���ؿ����ڤ�󧨤�����U�����R�O:

	karma init

�b�A���׺ݱ��������(�w���ؿ����,�M�����R�O), �L�|���ͤ@�ӵ������t�m���(`karma.conf.js`), �A�i�H�ھڧA���ߦn�ӽs�襦, ���q�{�a���@�ǫܦn���з�. �A�i�H�ϥΥ�.

**�Ұ�Karma���A��**

�u�ݭn�B��U�����R�O:

	karma start [optionalPathToConfigFile]

�o�N�|�b9876�ݤf�Ұ�Karma���A��(�o�O�q�{���p, �A�i�H�g�ѽs��b�W�@�B���쪺`karma.conf.js`���ӧ���). ���MKarma���ӥ��}�@���s�����æ۰ʮ���, ���N�b����x�����L�Ҧ���L�s����������һݭn�����O. �p�G�A�i�o�o�˰�, �u�ݭn�b��L�s�����Ϊ̳]�Ƥ��s��`http://localhost:9876`, �åB�A�̦n�b�h���s�������B�����.

> ���MKarma�i�H�۰ʮ���`�Ϊ��s����, �b�Ұʮ�.(FireFox, Chrome, IE, Opera, �ƦܬOPhantomJS), �������ȭ���u�O�o���s����. ����i�H�s���@��URL���]�Ƴ��i��i�H�@��Karma�B�澹. �]���p�G�A���}�A��iPhone�Ϊ�Android�]�ƤW�s�������s��`http://machinename:9876`(�u�n�O�i�X�ݪ�), �A���i��b���ʳ]�ƤW�B��P�˪�����.

**�B�����**

����U�����R�O:

	karma run

�N�O�o��. �B��o�өR�O����, �A������o���n���L�b����x�������G. ��²��, ���O��?

##�椸����

AngularJS�O���s�g�椸�����ܱo��²��, �q�{���p�U����s�g[Jasmine](http://pivotal.github.io/jasmine/)���檺����(�N�OKarma). Jasmine�N�O�ڭ̩һ����欰�X�ʶ}�o�ج[, �����\�A�s�g�W�d�ӻ����A���N�X�欰���Ӧp���{. �@��Jasmine���սd�Ҭݰ_�ӥi��O�o�ˤl��.

	describe("MyController:", function(){
		it("to work correctly", function(){
			var a = 12;
			var b = a;

			expect(a).toBe(b);
			expect(a).not.toBe(null);
		});
	});

���p�A�i�H�ݨ�, �������N�O�D�`�e���\Ū���榡, �j�������N�X���i�H��²�檺�^��Ӿ\Ū�z��. ���ٴ��ѤF�@�ӫD�`�h�ˤƩM�j�j���ǰt���X(�N��`expect`�q�y), ��M���٦�[xUnit](http://xunit.codeplex.com/)�`�Ϊ�`setUp`�M`tearDowns`(��Ʀb�C�ӿW�ߪ����եΨҤ��e�Ϊ̤������).

AngularJS���ѤF�@���u�����쫬, �M���ը�Ƥ@��, �����\�A���b�椸���դ��إߪA��, ����M�L�o�����v�Q, �H�μ���`HTTPRequests`��X����. �ڭ̱N�b�Ĥ����Q�׳o��.

Karma�i�H�ϥ��ܮe������X��A���}�o�y�{��, �H�Φb�A�s�g���N�X�����o�Y�ɪ����X.

**��X��IDEs��**

Karma�èS���Ҧ��̷s���M�̦n��(greatest)IDEs�ϥΪ�����(�w�g��{���٨S��), ����ڤW�A�ä��ݭn. �Ҧ��A�һݭn�����N�O�b�A��IDEs���K�[�@�Ӱ���"karma start"�M"karma run"���ֱ��R�O. �o�q�`�i�H�g�ѲK�[�@��²�檺�}���Ӱ���, �Ϊ̹�ڪ�shell�R�O, �̿��A�ҿ�ܪ��s�边. ��M, �C�������B��A�����Ӭݨ쵲�G.

**�b�C�@���ܤƤW�B�����**

�o�O�\�hTDD�}�o�̪��z�Q��: ����B��b���̩Ҧ������դ�, �C�����̫��U�O�s, �b��@�������t���o���^���G. �ϥ�AngularJS�MKarma�i�H�ܮe������o�@�I. �ƹ��ҩ�, Karma�t�m���(�O��N�O�e����`karma.conf.js`)���@�Ӭݦ��L�`���W��**`autoWatch`**���лx. �]�w����true�ӧi�DKarma�C���B��A�����դ��(�o�N�O�A����l�X�M���եN�X)���ʱ������ܤ�. �M��b�A��IDE������"karma start", �q�q�|���? Karma�B�浲�G�N�i�ѧA��IDE�ϥ�. �A�Ʀܤ��ݭn��������x�Ϊ̲׺ݨ��A�ѵo�ͤF����.

##�ݨ��/��X����

�H�����ε{�����o�i(�Ϊ̦��o���Ͷ�, �ƹ�W�ܧ�, ���e�A�Ʀܤw�g�N�Ѩ�o�@�I), ���ե��̬O�_�p�w�����ˤu�@�Ӥ��ݭn��ʪ����ť���\��. ����, �S�@�K�[�s���S��, �A���ȭn���ҷs�S�ʪ��u�@, �٭n���ҦѯS�ʬO�_���M������`�u�@, �åB�S��bug�M�\��]�S���h��. �p�G�A�}�l�K�[�h���s����, �A�i�H�ܮe�ݥX, ���o�ǥi�H�ܦ��@�ӲզX.

AngularJS���ϸg�Ѵ��Ѥ@��Scenario Runner�Ӽ����Τ�P���ε{���椬�ӽw�ѳo�ز{�H.

Scenario Runner���\�A������Jasmine���y�k�Ӵy�z���ε{��. ���p���e���椸����, �ڭ̱N�|���@�Ǫ�`describes`(�w��o�ӯS��), �P�ɥ��٬O�W��(�y�z�C�ӳ�W�\�઺�S��). �M���`�@��, �A�i�H���@�Ǧ@�P���欰, ������C�ӳW�d���e�M����.(�ڭ̺٤�������).

�Ӭݤ@�����ε{���d��, �L��^�L�o�����G�C��, �ݰ_�ӥi�๳�U���o��:

	describe("Search Results", function(){
		beforeEach(function(){
			browser().navigateTo("http://localhost:8000/app/index.html");
		});
		it("Should filter results", function(){
			input("searchBox").enter("jacksparrow");
			element(":button").click();
			expect(repeater("ul li").count()).toEqual(10);
			input("filterText").enter("Bees");
			expect(repeater("ul li").count()).toEqual(1);
		});
	});

����ؤ覡�B��o�Ǵ���. ���L, �L�רϥΨ��ؤ覡�B�楦��, �A���������@��Web���A���ӱҰʧA�����ε{���A��(�аѨ��W�@�`�Ӭd�ݦp�󰵨�o�@�I). �@������o�@�I, �i�H�ϥΤU�C��k���@:

1. **�۰ʤ�**: Karma�{�b����B��Angular��������. �إߤ@��Karma�t�m���M��i��H�U����:

  a. �K�[�@��ANGULAR_SCENARIO & ANGULAR_SCENARIO_ADAPTER��t�m����󳡤�.

  b. �K�[�@�ӥN�z���A���N�ШD�w��쥿�T�����դ��Ҧb�ؿ�, �Ҧp:

  	proxies = {'/': 'http://localhost:8000/test/e2e'};
  
  c. �K�[�@��Karma root(�ڥؿ�/��¦���|)�H�T�OKarma����l�X���|�z�Z�A������, ���o��:

  	urlRoot = '/_karma_/';

  �M��u�ݭn�O�o�g���s��`http://localhost:9876/_karma_`�Ӯ���Karma���A��, �A���Өϥ�Karma�ۥѪ��B��A������.

2. **���**: ��ʪ���k���\�A�q�A��Web���A���W���}�@��²�檺�����B��(�M�d��)�Ҧ�������.

  a. �إߤ@��²�檺`runner.html`���, �o�ӷ���Angular�w��`angular-scenario.js`���.

  b. �Ҧ���JS��l�X����`�A�ҽs�g���A�������ե󳡤����W�d.

  c. �ҰʧA��Web���A��, �s��`runner.html`���.

������A���Өϥ�Angular�����B�澹, �Ϊ̻��O�~�����ĤT��w���ݹ�ݪ����չB�澹? �ϥγ����B�澹���O�H��Y���n�B, �]�A:

**AngularJS�N��**

Angular�������B�澹, �U�W��q, ���O��Angular�إߪ�. �]��, �L�N�OAngular aware, ������òz�ѦU�ئU�˪�Angular����, �����j�w. �ݭn��J�@�Ǥ�r? �ˬd�j�w����? ���Ҥ��~��(repeater)���A? �Ҧ����o�ǳ��i�H�g�ѳ����B�澹���P������.

**�L���H������**

Angular�N�Ѥ]�N����Angular����Ҧ���XHR��ɦV���A����X, �q�ӥi�H�קK�����[���ҵ��ݪ����j�ɶ�. �����B�澹�����ɥ[���@�ӭ���, �q�Ӥ�Selenium���է��T�w��, �Ҧp, �W�ɵ��ݭ����[���ɥ��ȥi�ॢ��.

**�����\��** 

���sJavaScript, �p�G�A�d�ݧA���N�X���O�ܦn; ��A�Ʊ�Ȱ��M��_���ծ�, �Ҧ����o�ǳ��B��������ն�? �M�өҦ����o�@���g��Angular�����B�澹���O�i�檺, ����.

##�sĶ

�bJavaScript�@�ɸ�, �sĶ�q�`�N�������Y�N�X, ���M�@�ǹ�ڪ��sĶ�i��ϥΪ���Google��Closure�w. ���O����A�|�Ʊ�N�Ҧ��}�G��, �g���ܦn, �ܮe���z�ѥN�X�ܱo���iŪ�O?

��]���@�O�ڭ̪��ؼЬO�O���ε{����֪��^���Τ�. �o�O������Ȥ�����ε{���X�~�e���Q�{�b�˭��o�o��֪��D�n��]. ����V�����o���ε{���ùB��, �^���o�]�V��.

�o�اֳt�^���O���YJS�N�X���ʾ�. �N�X�V�p, �V�঳�Ī���p�t��, �P�ɯ����֪��N�������o�e���Τ�. �o�b�������ε{������o�׬����n, �]����W�Ҭ������~�V.

�o�̦�������k�i�H���Y�A�����ε{���ҽs�g��AngularJS�N�X, �C�ؤ�k���㦳���P���ĪG.

**�򥻪��M²�檺�u��**

�o�]�A���Y�Ҧ��b�A���N�X���ϥΪ��ܼ�, ���O���|���Y�ݩ�. �o�N�O�ҿת��ǻ���Closure Compiler��²���u��.

�̤��|���A�a�Ӧh�j�����j�p���`��, ���O�A���M�i�H��o�@�ӥi�[���̤p�}�P.

�o���u�@����]�O�sĶ��(Closure�Ϊ�UglifyJS)�ä��|���R�W�A�q�˪O���ޥΪ��ݩ�.  �]��, �A���˪O�|�~��u�@, �ȶȭ��R�W�ϰ��ܼƩM�Ѽ�.

���Google Closure, �u��²�檺�I�s�U�����R�O:

	java -jar closure_compiler.js --compilation_level | SIMPLE_OPTIMIZATIONS --js path/to/files.js

**�i���u��**

�i���u�Ʀ��@�I�Ƥ�, ���|�չϭ��W�X�G����F��M�C�Ө��. �o��o�ӯŧO���u�Ƥu�@, �A�N�ݭn�g����ܪ��i�D�����Ǩ��, �ܼƩM�ݩʻݭn���R�W(�g�ѨϥΤ@��externsfile). �̳q�`�O�g�Ѽ˪O�X�ݨ�ƩM�ݩ�.

�sĶ�N�|�ϥγo��`externs`���, �M�᭫�R�W�Ҧ����F��. �p�G�B�z�n, �o�i��|�ɭP���A��JavaScript���j�T�ת���p, ���O�����T�ݭn�۷�j���u�@��, �]�A�C�����ܥN�X���n���externs���.

�n�O��@���: ��A�Q�n���Y�N�X��, �A�n�ϥΨ̿�`�J���Φ�(�b����W���w`$inject`�ݩ�).

�U�����N�X���|�u�@

	function MyController($scope, $resource){
		//Stuff here
	}

�A�ݭn���U���o�˰�:

	function MyController($scope, $resource){
		//Some Stuff here
	}
	MyController.$inject = ['$scope', '$resource'];

�Ϊ̬O�ϥμҲ�, ���o��:

	myAppModule('MyController', ['$scope', '$resource', function($scope, $resource){
		//Some stuff here
	}]);

�@���Ҧ����ܼƳ��V�a�Ϊ����Y�u��, �o�O�ϥ�Angular��X���ǧA�̪�ϥΪ��A�ȩM�ܼƪ��覡.

> �C�����O�Ʋժ��覡�`�J�O����n���B�z�o�覡, �H�קK�}�l�sĶ�N�X�ɪ����~. ���Y�õ��ϧ�X�����򴣨Ѫ�$e�ܼƥᥢ�F(�@�ǥ��Ȫ��V�a�������Y�F��)�O���ȱo��.

##��L�u�q�u��

�b���`, �ڭ̱N�|�ݤ@�Ǩ�L���U��²�ƧA���}�o�y�{�M�����Ĳv���u��. �o�]�A�ϥ�Batarang�����u�ꪺ�N�X�M�ϥ�Yeoman�}�o.

###����

��A�ϥ�JavaScript�u�@��, �b�s�����������A���N�X�|�����@�ӲߺD. �A�V�������o�Өƹ�, ��A�V���n�B. �ȱo�y�����O, ��L�h�S��Firebug��, �o��Ƥw�g���L�F��������. �{�b, ���޿�ܤ����s����, �@��ӻ��A���i�H���J�N�X�Ӥ��R���~�M�P�_���ε{�������A. �u�ݭn�h�A��Chrome�MInternet Explorer���}�o�̤u��, ��P�ɦbFireFox�MChrome���u�@��Firebug.

�o�̦��@�����U�A�i�@�B�������ε{�����ޥ�����:

+ �û��O��, ��A�Ʊ氻���ޥε{�Ǯ�, �O�o������D���Y�������N�X�M�̿त�i��. �A���ȷ|��o��n(�iŪ)�ܼƦW, �]�|��o�N�X�渹�M��ڦ��Ϊ��T���H�ΰ����\��.
+ �ɶq�O���A����l�X���W�ߪ�JS���, �Ӥ��O���p�bHTML��.
+ �_�I�����O�ܦ��Ϊ�! ���̤��\�A�ˬd�A�����ε{�����A, �ҫ�, �H�ε��w���ɶ��I�W���Ҧ��T��.
+ "�Ȱ��Ҧ����`"�O���m�b���j�h�ƶ}�o�̤u�㤤���@�ӫD�`���Ϊ��ﶵ. ��o�{�@�Ӳ��`�O�������|�פ��~��B��ð��G�ɭP���`���N�X��.

###Batarang

��M, �ڭ̦�Batarang. Batarang�O�@�ӲK�[AngularJS���Ѫ�Chrome�X�R, ���O�O�M�bGoogle Chrome�����m�}�o�̤u��. �@���w��(�A�i�H�q[http://bit.ly/batarangjs](http://bit.ly/batarangjs)�����o), ���N�|�bChorme���}�o�̤u�㭱�O���K�[�@��AngularJS�ﶵ.

�A���S���Q�L�A��AngularJS���ε{������e���A�O����? ��e(����)�]�t���C�Ӽҫ�, �@�ΰ�M�ܼƬO����? �A�����ε{���ʯ�p��?  �p�G�A�٨S���Q�L, �۫H��, �A�|��. ��A�ݭn�o�򰵮�, Batarang�|���A�A��.

�o�̦�Batarang���|�ӥD�n�����Ϊ����[�\��:

####�ҫ��ﶵ

Batarang���\�A�q�ڷ��V�U�`�J���s`scope`. �M��A�i�H�ݨ�o��`scopes`�O�p��O�M�H�μҫ��O�p��P�����p��.(�p��3-2�ҥ�). �A�Ʀܥi�H��ɪ����ܥ��̨æb���ε{�����d���ܤƪ��ϬM. �ܻ�, ���O��?

![model tab](figure/3-2.png)

Figure 3-2 Model tree in Batarang

####�ʯ�ﶵ

�ʯ�ﶵ������W�ҥ�, ���|�`�J�@�ǯS��JavaScript�N�X��A�����ε{����. �@���A�ҥΥ�, �A�N�i�H�ݨ줣�P���@�ΰ�M�ҫ�, �åB�i�H�b�C�ӧ@�ΰ����Ҧ����ʯ�ʱ���F��(�p��3-3�ҥ�). �H�ۧA�ϥ����ε{��, �ʯ�]�|�o���s, �]�����i�H�ܦn����ɤu�@.

![perforemance tab](figure/3-3.png)

Figure 3-3. Performance tab in Batarang

####�A�Ȩ̿�

���@��²�檺���ε{��, ���|�W�L1-2�ӱ���M�A�Ȩ̿�. ���O�ƹ�W, ���������ε{��, �p�G�S���u����, �A�Ȩ̿�޲z�|��������. ���n�o�̦�Batarang�i�H���A���ѪA��, ��ɳo�Ӭ}, �]�������A���ѤF�@�Ӱ��b, ²�檺��k�Ӭd�ݥi���ƪ��A�Ȩ̿�Ϫ�(�p��3-4�ҥ�).

![service dependencies](figure/3-4.png)

Figure 3-4. Charting dependencies in Batarang

####�����ݩʩM����x�X��

��A�g��HTML�˪O�ӱ��s�@��AngularJS���ε{����, �����ﶵ���ݩʵ��椤�{�b���@���B�~��AngularJS�ݩʳ���. �o���\�A�ˬd�ҫ��ҳs�������w������`scope`. ���]�|���}�o�Ӥ�����`scope`�챱��x��, �]���A�i�H�b����x���g��`$scope`�ܼƨӳX�ݥ�. �p��3-5�ҥ�:

![properties](figure/3-5.png)

Figure 3-5. AngularJS properties within Batarang

##Yeoman: �u�ƧA���u�@�y�{

�۷�h���u��p�B��K�����{, �H���U�A�b�}�o���ε{�����u�Ƥu�@�y�{. �ڭ̦b�e�����`�ҽͤΪ�Yeoman�N�O�o�ˤ@�ؤu��, ���֦��O�H�L�H�`�誺�\�ධ, �]�A:

+ ���֪��}��[
+ ���m�w�����A��
+ ��X�]�޲z
+ �@�y���c�عL�{
+ �ϥ�PhantomJS�i��椸����

���٫ܦn����X�M�X�R�FAngularJS, �o�]�O�ڭ̬�����j�P���˥���AngularJS���بϥΥ����D�n��]���@. ���ڭ̸g�ѤW���������覡�ϥ�Yeoman�ɧA���ͬ����P.

###�w��Yeoman

�w��Yeoman�O�@�Ӭ۷�������L�{, ���]�i�H�g�Ѥ@�Ǹ}�������U�A�w��.

�bMac/Linux�����W, �B��U�����R�O:

	curl -L get .yeoman.io | bash

�M��u�ݫ��ӥ��L���u�O�Ө��oYeoman.

���Windows����, �Ϊ̹B�楦�O�J�������D, ��[https://github.com/yeoman/yeoman/ wiki/Manual-Install](https://github.com/yeoman/yeoman/ wiki/Manual-Install)�ë��ӻ����Ӧw�˷|���A�Z�q�L��.

###�Ұʤ@�ӷs��AngularJS����

���p�e���Ҵ��쪺, �Ʀܤ@��²�檺���س����\�h�޳N�ݭn�B�z, �q�˪O���¦����, �A��w�̿�, �@���Ʊ����ݭn���c��. �A�i�H��ʪ����o�Ǥu�@, �Ϊ̤]�i�H�ϥ�Yeoman�B�z��.

�u�ݬ��A�����ؤ�²�檺�إߤ@�ӥؿ�(Yeoman�N��ؿ��W�ٷ�@���ئW��), �M��B��U�����R�O:

	yeoman init angular

�o�N�إߤ@�ӥ��������u�Ƴ����ҸԲӴy�z���@�ӧ��㪺���c, �]�A��V���Ѫ��ج[, �椸���յ���.

###�B����A��

�p�G�A���A��Yeoman, ����A���o���إߤ@��HTTP���A���ӪA�ȧA���e�ݥN�X. ���O�p�G�ϥ�Yeoman, ����A�N��o�@�Ӥ��m���w���t�m�n�����A���åB�ٯ���o�@���B�~���n�B. �A�i�H�ϥΤU�����R�O�Ұʦ��A��:

	yeoman server

�o�����u�Ұʤ@��Web���A���ӪA�ȩ�A���N�X, ���ٷ|�۰ʥ��}�A��Web�s�����æb�A���ܧA�����ε{���ɨ�s�A���s����.

###�K�[�s������, ���ϩM���

�K�[�@�ӷs��Angular���ѯA�Φh�ӨB�J, �䤤�]�A:

+ �b`index.html`���ҥηs�����JS���
+ �K�[���T�����Ѩ�AngularJS�Ҳդ�
+ �إ�HTML�˪O
+ �K�[�椸����

�Ҧ����o�ǦbYeoman���ϥΤU�����R�O�i�H�b�@�B����:

	yeoman init angular:route routeName

�]��, �p�G�A�B��`yeoman iniy angular route home`�������ᥦ�N����H�U�ާ@:

+ �b`app/scripts/controllers`�ؿ����إߤ@��`home.js`������[
+ �b`test/specs/controllers`�ؿ����إߤ@��`home.js`���ճW�d
+ �N`home.html`�˪O�K�[��`app/views`�ؿ���
+ �챵�D�ޥμҲդ���home����(�bapp/scripts/app.js`���)

�Ҧ����o�ǳ��u�ݭn�@����W���R�O!

###���ժ��G��

�ڭ̤w�g�ݹL�ϥ�Karma�p���P���ҰʩM�B�����. �̲�, �B��Ҧ����椸���եu�ݭn����R�O.

Yeoman�ϥ��ܱo��e��(�p�G�A�۫H��). �C��A�ϥ�Yeoman���ͤ@�Ӥ��, �����|���A�إߤ@�Ӷ�R�������զs��. �@���A�w�ˤFKarma, �ϥ�Yeoman�B����եu�ݰ���U�����R�O�Y�i:

	yeoman test

###�c�ض���

�c�ؤ@�ӧ��ƪ����ε{���i��O�h�W��, �Ϊ̦ܤ֯A�Ψ�ݭn�B�J. Yeoman�g�Ѥ��\�A���U���o�˰���F���ֵh�W:

+ �s��(�X��)�Ҧ�JS�}����@�Ӥ��
+ �����Ƥ��
+ �u�ƹϤ�
+ �������ε{���֨��M��

�Ҧ����o�Ǧn�B���Ӧ۩�@���R�O:

	yeoman build

Yeoman��������Y���, ���O�ھڨӵo�̴��Ѫ��T��, ���ܧַ|���.

##�ϥ�RequireJS��XAngularJS

�p�G�A���氵�n��h���Ʊ�, ���n�|���A���}�o���ҧ�²��. ����ק�A���}�o����, �|�ݭn�ק��h�����. �̿�޲z�M�إߥ]���p�O����W�Ҫ����ةҼ~�{��.

�ϥ�JavaScript�]�w�A���}�o���ҬO�۷�x����, �]�����A��Ant�c�غ��@, �s���A�����Ӻc�ظ}��, ���Y���̵���. �ȱo�y�����O, �b���[���e�w�g�X�{�F��RequireJS�o�˪��u��, �����\�A�w�q�M�޲z�A��JS�̿����Y, �H�αN�L�̱���@��²�檺�c�عL�{��. �H�۳o�ǫD�P�B�[���޲z���u��ϥ�, ����T�O�Ҧ����̿���b���椧�e�[���n, ���I�u�@�i�H��b��ڪ��\��}�o, �b�����e�q���p��²��L.

�ȱo�y�����O, AngularJS����ܦn���o��[RequireJS](http://requirejs.org/), �]���A�i�H���������. �o�̦��@�ӥؼнd��, �ڭ̧��F�b�@�Өt�Τ�����u�@���ܦn�ӥB�����`���覡�Ӵ��Ѥ@�Ӽ˥��]�w.

���ڭ̤@�_�Ӭݬݳo�Ӷ��ت���´(�����e���y�z�����[, �y�L���@�I�ܤ�):

1. **app**: �o�ӥؿ��O�Ҧ���ܵ��Τ᪺���ε{���N�X�J�D�ؿ�. �]�AHTML, JS, CSS, �Ϥ��M�̿઺�禡�w.

    a. /**style**: �]�t�Ҧ���CSS/Less���

    b. /**images**: �]�t���ت��Ҧ��Ϥ����

    c. /**script**: �DAngularJS�N�X�w. �o�ӥؿ��]�]�A�ڭ̪��޾ɵ{�ǥN�X, �D�n��RequireJS��X

        i. /**controllers**: �o�̬OAngularJS���
        
        ii. /**directives**: �o�̬OAngularJS���O

        iii. /**filters**: �o�̬OAngularJS�L�o��

        iv. /**services**: �o�̬OAngularJS�A��

    d. /**vendor**: �ڭ̩Ҩ̿઺�禡�w(Bootstrap, RequireJS, jQuery)

    e. /**views**: ���Ϫ�HTML�˪O�����M���ةҨϥΪ��ե�

2. **config**: �]�t�椸���թM�������ժ�Karma�t�m

3. **test**: �]�t���ε{�����椸���թM��������(��X��)

    a. /**spec**: �]�t���ε{����JS�ؿ������椸���թM�蹳���c

    b. /**e2e**: �]�t�ݨ�ݪ������W�d

�ڭ̩һݭn�����Ĥ@��Ʊ��O�b`main.js`���(�bapp�ؿ�)���ޤJRequireJS, �M��ϥΥ��[���Ҧ�����L�̿ඵ. �o�̦��@�ӨҤl, �ڭ̪�JS���ذ��F�ۤv���N�X�ٷ|�̿��jQuery�MTwitter��Bootstrap.

	//the app/scripts/main.js file, which defines our RequireJS config
	require.config({
		paths: {
			angular: 'vendor/angular.min',
			jquery: 'vendor/jquery',
			domReady: 'vendor/require/domReady',
			twitter: 'vendor/bootstrap',
			angularResource: 'vendor/angular-resource.min'
		},
		shim: {
			'twitter/js/bootstrap': {
				deps: ['jquery/jquery']
			},
			angular: {
				deps: ['jquery/jquery', 'twitter/js/bootstrap'],
				exports: 'angular'
			},
			angularResource: {
				deps: ['angular']
			}
		}
	});

	require([
		'app',
		//Note this is not Twitter Bootstrap
		//but our AngularJS bootstrap
		'bootstrap',
		'controllers/mainControllers',
		'services/searchServices',
		'directives/ngbkFocus'
		//Any individual controller, service, directive or filter file
		//that you add will need to be pulled in here.
		//This will have to be maintained by hand.
		],
		function(angular, app){
			'use strict';

			app.config(['$routeProvider',
				function($routeProvider){
					//define your Routes here
				}
			]);
		}
	);

�M��ڭ̩w�q�@��`app.js`���. �o�Ӥ��w�q�ڭ̪�AngularJS���ε{��, �P�ɧi�D��, ���̿��ڭ̩ҩw�q���Ҧ����, �A��, �L�o���M���O. �ڭ̩Ҭݨ쪺RequireJS�̿�C���Ҵ��쪺�u�O�@�I�I.

�A�i�H�{��RequireJS�̿�C��N�O�@��JavaScript��import�y�y��. �]�N�O��, �N�X��������ƪ���Ҧ����̿�C�������Ϊ̥[�������������|����.

�t�~�Ъ`�N, �ڭ̤��|��W �i�DRequireJS, ���J������,�A�ȩΪ̹L�o���O����, �]���o�Ǩä��ݩ󶵥ت����c. �C�ӱ��, �A��, �L�o���M���O���O�@�ӼҲ�, �]���u�w�q�o�Ǭ��ڭ̪��̿�N�i�H�F.

	// The app/scripts/app.js file, which defines our AngularJS app
	define(['angular', 'angularResource', 'controllers/controllers','services/services', 'filters/filters','directives/directives'],function (angular) {
		return angular.module(�yMyApp�z, ['ngResource', 'controllers', 'services','filters', 'directives']);
	});

�ڭ��٦��@��`bootstrap.js`���, ���쵥��DOM�ǳƴN��(�o�̨ϥΪ�RequireJS������`domReady`), �M��i�DAngularJS�~�����, �o�O�ܦn��.

	// The app/scripts/bootstrap.js file which tells AngularJS
	// to go ahead and bootstrap when the DOM is loaded
	define(['angular', 'domReady'], function(angular, domReady) {
		domReady(function() {
			angular.bootstrap(document, [�yMyApp�z]);
		});
	});

�o�̱N�޾ɱq���ε{�������ΥX��, �٦��@�Ӧ���, �Y�ڭ̥i�H�ϥΤ@�Ӱ��y������b�����N�ڭ̪�`mainApp`�Ϊ̥X����ժ��ت��ϥΤ@��`mockApp`. �Ҧp �p�G�A�Ҩ̿઺���A�����i�}, �A�u�ݭn�إߤ@��`fakeApp`�ϥΰ��y����ƨӴ����Ҧ���`$http`�ШD, �H�O���A���}�o����. �o�˪���, �A�N�i�H�u�������ϥΤ@��`fakeBootstrap`�M�@��`fakeApp`��A�����ε{����.

�{�b, �A��`main.html`�D�˪O(app�ؿ���)�i��ݰ_�ӹ��U���o��:

	<!DOCTYPE html>
	<html> <!-- Do not add ng-app here as we bootstrap AngularJS manually-->
	<head>
		<title>My AngularJS App</title>
		<meta charset="utf-8" />
		<link rel="stylesheet" type="text/css" href="styles/bootstrap.min.css">
		<link rel="stylesheet" type="text/css"
		href="styles/bootstrap-responsive.min.css">
		<link rel="stylesheet" type="text/css" href="styles/app.css">
	</head>
	<body class="home-page" ng-control ler="RootController">
		<div ng-view ></div>
		<script data-main="scripts/main" src="lib/require/require.min.js"></script>
	</body>
	</html>

�{�b, �ڭ̨Ӭݬ�`js/controllers/controllers.js`���, �o�ݰ_�ӴX�G�P`js/directives/directives.js`, `js/filters/filters.js`�M`js/services/services.js`�@�Ҥ@��:

	define(['angular'], function(angular){
		'use strict';
		return angular.module('controllers', []);
	});

�]���ڭ̨ϥΤFRequireJS�̿઺���c, �Ҧ����o�ǳ��|�O�ҥu�bAngular�̿ມ���å[�����������p�U�~�|�B��.

�C�Ӥ�󳣩w�q���@��Angular�Ҳ�, �M��g�ѱN��Ӫ����, ���O, �L�o���M�A�ȲK�[��w�q���Өϥ�.

���ڭ̨Ӭݬݤ@�ӫ��w�w�q(��p�ĤG����`focus`���O):

	//File: ngbkFocus.js

	define(['directives/directives'], function(directives) {
		directives.directive(ngbkFocus, ['$rootScope'], function($rootScope){
			return {
				restict: 'A',
				scope: true,
				link: function(scope, element, attrs){
					element[0].focus();
				}
			}
		});
	});

���O�ۤ���ܺ��H��, ���ڭ̥J�Ӭݬݵo�ͤF����. ��¶�ۤ��RequireJS shim�i�D�ڭ�`ngbkFocus.js`�̿��b�Ҳդ��n����`directices/directives.js`���. �M�ᥦ�ϥΪ`�J���O�ҲձN�ۨ����O�n���K�[�i��. �A�i�H��ܦh�ӫ��O�Ϊ̤@�ӳ�@�����������. �o�����ѧA�M�w.

�@�ӭ��I���`�N�ƶ�: �p�G�A���@�ӱ���i�J��A�Ȥ�(�]�N�O���A��`RootController`�̿��A��`UserSevice`, �åB���o`UserService`�`�J), ����A�����T�O�N�A�w�q�����[�JRequireJS�̿त, �N���o��:

	define(['controllers/controllers', 'services/userService'], function(controllers){
		controllers.controller('RootController', ['$scope', 'UserService', function($scope, UserService){
			//Do what's needed
		}]);
	});

�o�򥻤W�O�A��ӭ�l�X�ؿ������c�]�w.

���O�A�|��, �o�p��B�z�ڪ�����? �ګܰ����A�|�ݳo�Ӱ��D, �]���A�|�o�쵪��.

���ӫܦn������, Karma���RequireJS. �u�ݦw�˳̷s�M�̦n������Karma.(�ϥ�`npm install -g karma`).

�@���A�w�˦nKarma, Karma�w��椸���ժ��t�m�]�|�^��������. �H�U�O�ڭ̦p�G�]�w�ڭ̪��椸���ըӹB��ڭ̤��e�w�q�����ص��c:

    // This file is config/karma.conf.js.
    // Base path, that will be used to resolve files
    // (in this case is the root of the project)
    basePath = '../';

    // list files/patterns to load in the browser
    files = [
        JASMINE,
        JASM I NE_ADAPTER
        REQUIRE,
        REQU I RE_ADAPTER ,
        // !! Put all libs in RequireJS 'paths' config here (included: false).
        // All these files are files that are needed for the tests to run,
        // but Karma is being told explicitly to avoid loading them, as they
        // will be loaded by RequireJS when the main module is loaded.
        {pattern: 'app/scripts/vendor/**/*.js', included: false},
        // all the sources, tests // !! all src and test modules (included: false)
        {pattern: 'app/scripts/**/*.js', included: false},
        {pattern: 'app/scripts/*.js', included: false},
        {pattern: 'test/spec/*.js', included: false},
        {pattern: 'test/spec/**/*.js', included: false},
        // !! test main require module last
        'test/spec/main.js'
     ];
    // list of files to exclude
    exclude = [];

    // test results reporter to use
    // possible values: dots || progress
    reporter = 'progress';

    // web server port
    port = 8989;
    
    // cli runner port
    runnerPort = 9898;

    // enable/disable colors in the output (reporters and logs)
    colors = true;

    // level of logging
    logLevel = LOG_INFO;

    // enable/disable watching file and executing tests whenever any file changes
    autoWatch = true;

    // Start these browsers, currently available: 
    // - Chrome
    // - ChromeCanary
    // - Firefox
    // - Opera
    // - Safari
    // - PhantomJS
    // - IE if you have a windows box 
    browsers = ['Chrome'];
    
    // Cont inuous Integrat ion mode
    // if true, it captures browsers, runs tests, and exits 
    singleRun = false;

 �ڭ̨ϥΤ@�ӵy�L���P���榡�өw�q���ڭ̪��̿�(�]�A: false�O�D�`���n��). �ڭ��ٲK�[�FREQUIRE_JS�M�A�t�̿�. �̲׶i��o�@�t�C�u�@���O`main.js`, �L�|Ĳ�o�ڭ̪�����.

	// This file is test/spec/main.js

	require.config({
		// !! Karma serves files from '/base'
		// (in this case, it is the root of the project /your-project/app/js) 
		baseUrl: ' /base/app/scr ipts' ,
		paths: {
        angular: 'vendor/angular/angular.min',
			jquery: 'vendor/jquery',
			domReady: 'vendor/require/domReady',
			twitter: 'vendor/bootstrap',
			angularMocks: 'vendor/angular-mocks',
			angularResource: 'vendor/angular-resource.min',
			unitTest: '../../../base/test/spec'
		},

		// example of using shim, to load non-AMD libraries
		// (such as Backbone, jQuery)
		shim: {
			angular: {
				exports: 'angular'
			},
			angularResource: { deps:['angular']},
			angularMocks: { deps:['angularResource']}
		}
	});

	// Start karma once the dom is ready.
	require([
        'domReady' ,
        // Each individual test file will have to be added to this list to ensure
        // that it gets run. Again, this will have to be maintained manually.
        'unitTest/controllers/mainControllersSpec',
        'unitTest/directives/ngbkFocusSpec',
        'unitTest/services/userServiceSpec'
        ], function(domReady) {
            domReady(function() {
                window.__karma__.start();
        });
    });

�Ѧ��]�w, �ڭ̥i�H�B��U�����R�O

	karma start config/karma.conf.js

�M��ڭ̴N�i�H�B����դF.

��M, ���A�Ψ�s�g�椸���մN�ݭn�y�L�����ܤ@�U. ���̻ݭnRequireJS������Ҳ�, �]�����ڭ̨Ӭݤ@�Ӵ��սd��:

	// This is test/spec/directives/ngbkFocus.js
	define(['angularMocks', 'directives/directives', 'directives/ngbkFocus'], function() {
		describe('ngbkFocus Directive', function() {
			beforeEach(module('directives'));

			// These will be initialized before each spec (each it(), that is),
			// and reused
			var elem;
			beforeEach(inject(function($rootScope, $compile) {
				elem = $compi le('<input type=�vtext�v ngbk-focus>')($rootScope);
			}));

			it('should have focus immediately', function() { 
				expect(elem.hasClass('focus')).toBeTruthy();
			});
		});
	});

�ڭ̪��C�Ӵ��ձN����H�U�X�I:

1. �Ԩ�`angularMocks`���o�ڭ̪�angular, angularResource, ��M�٦�angularMocks.

2. �Ԩ��i���Ҳ�(directives�������O, controllers�����������), �M�ᥦ��ڤW���ժ��O��W�����(loadingIndicator).

3. �p�G�A�����շU�ӷU��L���A�ȩΪ̱��, ���F�bAngularJS���i���N�~, �n�T�O�]�w�q�bRequireJS���̿त.

�o�ؤ�k�i�H�Ω�������, �ӥB�A���ӳo��.

�ȱo�y�����O, RequireJS���B�z�覡�ä��|�v�T�ڭ̩Ҧ����ݨ�ݪ�����, �]���i�H�ϥΧڭ̥ثe�Ҭݨ쪺�覡²�檺����o�@�I. �@�ӽd�Ұt�m�p�U, ���]�A���A�Ȩ�bhttp://localhost:8000�W�B��A�����ε{��:

	// base path, that will be used to resolve files
	// (in this case is the root of the project 
	basePath = '../';

	// list of files / patterns to load in the browser
	files = [
		ANGULAR_SCENARIO,
		ANGULAR_SCENARIO_ADAPTER,
		'test/e2e/*.js'
	];

	// list of files to exclude
	exclude = [];

	// test results reporter to use
	// possible values: dots || progress
	reporter = 'progress';

	// web server port
	port = 8989;

	// cli runner port
	runnerPort = 9898;
	
	// enable/disable colors in the output (reporters and logs)
	colors = true;

	// level of logging
	logLevel = LOG_INFO;

	// enable/disable watching file and executing tests whenever any file changes
	autoWatch = true;

	urlRoot = '/_karma_/';

	proxies = {
		'/': 'http://localhost:8000/'
	};

	// Start these browsers, currently available:
	browsers = ['Chrome'];

	// Cont inuous Integrat ion mode
	// if true, it capture browsers, run tests and exit
	singleRun = false;
