#���R�@��AngularJS���ε{��

�b��2����, �ڭ̤w�g�Q�פF�@��AngularJS�`�Ϊ��\��, �M��b��3���Q�פF�Ӧp�󵲺c�ƶ}�o���ε{��. �{�b, �ڭ̤��A�~��`��Ӫ��޳N�I, ��4���N�۲���@�Ӥp��, ��ڪ����ε{���i������. �ڭ̱N�q�@�ӹ�ڦ��Ī����ε{�����P���@�U�ڭ̤��e�w�g�Q�׹L��(�d��)�Ҧ�������.

�ڭ̱N�C�����Ф@����, �M��Q�ר䤤����M���p������, �Ӥ��O�Q�ק������ε{�����e�ݩM�֤�, �̫�b�������᭱�ڭ̷|�C�C²���o�ӧ��㪺���ε{��.

##���ε{��

Guthub�O�@��²�檺���к޲z����, �ڭ̳]�p���Ω�s�x�ڭ̶W�ŨS��������, �P�ɮi��AngularJS���ε{�����U�Ӥ��P������. �o�����ε{���]�t�H�U���e:

+ �@�Ө��檺���p
+ �b�������@�Ӿɯ���
+ ���\�A�إ߷s������
+ ���\�A�s���{�������ЦC��

�D���Ϧb����, ���ܤƨ̿��URL, �Ϊ̭��ЦC��, �Ϊ̳�ӭ��Ъ��Ա�, �Ϊ̥i�K�[�s���Ъ��s��\��, �Ϊ̽s��{��������. �ڭ̥i�H�b��4-1���ݨ�o�����Ϊ��@�ӺI��:

![Guthub](figure/4-1.png)

Figure 4-1. Guthub: A simple recipe management application

�o�ӧ��㪺���ε{���i�H�b�ڭ̪�Github����`chapter4/guthub`���o��.

##�ҫ�, ����M�˪O���������Y

�b�ڭ̲`�J���ε{�����e, ���ڭ̨Ӫ�@��q��r�ӰQ�ץH�U�p��N���D�����̤T�����b���ε{������´�b�@�_�u�@, �P�ɨӫ�Ҥ@�U�䤤���C�@����.

`model`(�ҫ�)�O�u�z. �u�ݭn���Ƴo�y�ܴX��. ������ε{����ܤ���, �p����ܦb���Ϥ�, �O�s����, �����@�����|���ҫ����v�T. �]���A�n�B�~��@�Ǯɶ��ӫ�ҧA���ҫ�, ��H���ݩʱN�O����, �H�ΧA����p��q���A�����o�ëO�s��. ���ϱN�g�Ѹ��ô�����覡�۰ʧ�s, �ҥH�ڭ̪��J�I���Ӷ����b�ҫ��W.

`controller`�O�s�~���޿�: �p����o�ҫ�, ���椰��˪��ާ@, ���ϻݭn�q�ҫ������o����˪��T��, �H�Φp��N�ҫ��ഫ���A�ҷQ�n��. ����¾�d, �ϥΩI�s���A��, �޾ɧA�����ϨϥΥ��T�����, �j�h�Ʊ��p�U�Ҧ����o�ǨƱ����ݩ󱱨�ӳB�z.

�̫�, `template`�N��A���ҫ��N�p�����, �H�ΥΤ�N�p��P�A�����ε{���椬. ���D�n�����H�U�X�I:

+ ��ܼҫ�
+ �w�q�Τ�i�H�P�A�����ε{���椬���覡(�I��, ��r��J����)
+ ���ε{�����˦�, �ýT�w��ɥH�Φp����ܤ@�Ǥ���(��ܩ�����, hover����)
+ �L�o�M�榡�Ƹ��(�]�A��J�M��X)

�n�N�Ѩ�bAngular�����ҫ�-����-����A�μҦ����˪O�ä��O���n������. ����, ���ϬO�˪O���o����Q�sĶ�᪺����. ���O�@�Ӽ˪O�M�ҫ����զX.

�����������~���޿�M�欰�������Ӷi�J�˪O��; �o�ǰT�����ӳQ����b�����. �O���˪O��²��i�H�A���������`�I, �åB�i�H�T�O�A�u�ϥγ椸���ժ����p�U�N������դj�h�ƪ��N�X. �Ӽ˪O�����ϥγ������ժ��覡�Ӵ���.

���O, �A�i��|��, �b���̾ާ@DOM�O? DOM�ާ@�ä��|�u���i�J�챱��M�˪O��. ���|�s�b��Angular�����O��(���ɭԤ]�i�H�g�ѪA�ȨӳB�z, �o�˥i�H�קK���ƪ�DOM�ާ@�N�X). �ڭ̷|�b�ڭ̪�GutHub���d�Ҥ�󤤲[�\�@�ӳo�˪��Ҥl.

�o�ܤֻ�, ���ڭ̨Ӳ`�J���Q�@�U����.

##�ҫ�

������ε{���ڭ̭n�O���ҫ��D�`²��. �o�@���@�ӵ���. �b��ӧ��㪺���ε{����, ���̬O�@�Ӱߤ@���ҫ�. ���O�c�ؤ@������¦.

�C�ӵ��г����U�����ݩ�:

+ �@�ӥΩ�O�s����A����ID
+ �@�ӦW��
+ �@��²�u���y�z
+ �@�Ӳi������
+ �O�_�O�@�ӯS�⪺����
+ �@�Ӧ����Ʋ�, �C�Ӧ������ƶq, ���M�W��

�N�O�o��. �D�`²��. ���ε{�������@�������o��²�檺�ҫ�. �U���O�@�����A���Ϊ��d�ҵ���(�p��4-1�@��):

	{
		'id': '1',
		'title': 'Cookies',
		'description': 'Delicious. crisp on the outside, chewy' +
			' on the outside, oozing with chocolatey goodness' +
			' cookies. The best kind',
		'ingredients': [
			{
				'amount': '1',
				'amountUnits': 'packet',
				'ingredientName': 'Chips Ahoy'
			}
		],
		'instructions': '1. Go buy a packet of Chips Ahoy\n'+
			'2. Heat it up in an oven\n' +
			'3. Enjoy warm cookies\n' +
			'4. Learn how to bake cookies from somewhere else'
	}

�U���ڭ̱N�|�ݨ�p����o��²�檺�ҫ��c�ا������UI�S��.

##���, ���O�M�A��

�{�b�ڭ̲ש�i�H�o��o�����ڭ̤������r��׸̭��h���������ε{���F. ����, �ڭ̨ӬݬݥN�X�������O�M�A��, �H�ΰQ�ץH�U���̳��O������, �M��ڭ̧ڭ̷|�ݬݳo�����ε{���ݭn���h�ӱ��.

###�A��

	//this file is app/scripts/services/services.js

	var services = angular.module('guthub.services', ['ngResource']);

	services.factory('Recipe', ['$resource', function(){
		return $resource('/recipes/:id', {id: '@id'});
	}]);

	services.factory('MultiRecipeLoader', ['Recipe', '$q', function(Recipe, q){
		return function(){
			var delay = $.defer();
			Recipe.query(function(recipes){
				delay.resolve(recipes);
			}, function(){
				delay.reject('Unable to fetch recipes');
			});
			return delay.promise;
		};
	}]);

	services.factory('RecipeLoader', ['Recipe', '$route', '$q', function(Recipe, $route, $q){
		return function(){
			var delay = $q.defer();
			Recipe.get({id: $route.current.params.recipeId}, function(recipe){
				delay.resolve(recipe);
			}, function(){
				delay.reject('Unable to fetch recipe' + $route.current.params.recipeId);
			});
			return delay.promise;
		};
	}]);

�������ڭ̨Ӭݬݧڭ̪��A��. �b33����"�ϥμҲղ�´�̿�"�p�`���w�g�A�Ψ�F�A�Ȭ���������. �o��, �ڭ̱N�|��`�@�I�����A�Ȭ������T��.

�b�o�Ӥ��, �ڭ̹�ҤƤF�T��AngularJS�A��.

���@�ӵ��ЪA��, ����^�ڭ̩ҩI�s��Angular Resource. �o�ǬORESTful�귽, �����V�@��RESTful���A��. Angular Resource�ʸˤF�C�h��`$http`�A��, �]���A�i�H�b�A���N�X���u�B�z�ﹳ.

�`�N��W������N�X - `return $resource` - (��M, �̿��`guthub.services`�ҫ�), �{�b�ڭ̥i�H�N`recipe`�@���Ѽƶǻ������N�������, ���N�|�`�J�챱���. ���~, �C�ӵ��й�H�����m�����H�U�X�Ӥ�k:

+ Recipe.get()
+ Recipe.save()
+ Recipe.query()
+ Recipe.remove()
+ Recipe.delete()

> �p�G�A�ϥΤF`Recipe.delete`��k, �åB�Ʊ�A�����ε{���u�@�bIE��, �A���ӹ��o�˩I�s��: `Recipe[delete]()`. �o�O�]���bIE��`delete`�O�@������r.

���W������k, �Ҧ����d�߲��h���b�@�ӳ�W�����Ф��i��; �q�{���p�U`query()`��^�@�ӵ��мƲ�.

`return $resource`�o��N�X�Ω��n���귽 - �]���F�ڭ̤@�Ǧn�F��:

1. �`�N: URL����id�O���w��RESTFul�귽. ���򥻤W�O��, ��A�i�����d�߮�(`Recipe.get()`), �p�G�A�����ǻ��@��id�r�q, ����o�Ӧr�q���ȱN�Q�K�[��URL������.

�]�N�O��, �I�s`Recipe.get{id: 15})�N�|�ШD/recipe/15.

2. ���ĤG�ӹ�H�O����O? {id: @id}��? �O��, ���p�L�̩һ���, �@��N�X�i��ݭn�@�d�����, �������ڭ��|�@��²�檺�Ҥl.

��軡�ڭ̦��@��recipe�ﹳ, �䤤�s�x�F���n���T��, �åB�]�t�@��id.

�M��, �ڭ̥u�ݭn���U���o�˰��N�i�H�O�s��:

	//Assuming existingRecipeObj has all the necessary fields,
	//including id(say 13)
	var recipe = new Recipe(existingRecipeObj);
	recipe.$save();

�o�N�|Ĳ�o�@��POST�ШD��`/recipe/13`.

`@id`�Ω�i�D��, �o�̪�id�r�q���ۥ�����H���P�ɥΩ�@��id�Ѽ�. �o�O�@�Ӫ��[���K�Q�ާ@, �i�H�`�ٴX��N�X.

�b`apps/scripts/services/services.js`������Ө�L���A��. ���̨�ӳ��O�[����(Loaders); �@�ӥΩ�[����W������(RecipeLoader), �t�@�ӥΩ�[���Ҧ�������(MultiRecipeLoader). �o�b�ڭ̳s����ڭ̪����Ѯɨϥ�. �b�֤ߤW, ���̨�Ӫ�{�o�D�`�ۦ�. �o��ӪA�Ȧp�U:

1. �إߤ@��`$q`����(deferred)�ﹳ(���̬OAngularJS��promises, �Ω��챵�D�P�B���).
2. �إߤ@�Ӧ��A���I�s.
3. �b���A����^�Ȯ�resolve����ﹳ.
4. �g�Ѩϥ�AngularJS�����Ѿ����^promise.

> **AngularJS����Promises**
>
> �@��promise�N�O�@�Ӧb���ӬY�Ӯɨ�B�z��^�ﹳ�Ϊ̶�R�������f(�򥻤W���O�D�P�B�欰). �q�֤ߤW��, �@��promise�N�O�@�ӱa��`then()`���(��k)����H.
>
>���ڭ̨ϥΤ@�ӨҤl�Ӯi�ܥ����u��, ���]�ڭ̻ݭn���o�@�ӥΤ᪺��e�t�m:

	var currentProfile = null;
	var username = 'something';

	fetchServerConfig(function(){
		fetchUserProfiles(serverConfig.USER_PROFILES, username, 
			function(profiles){
				currentProfile = profiles.currentProfile;	
		});	
	});

> ���o�ذ��k�o�̦��@�ǰ��D:
>
> 1. ���̫Უ�ͪ��N�X, �Y�i�O�@�Ӿ���, �S�O�O�p�G�A�n�챵�h�өI�s��.
> 
> 2. �b�^�I�M��Ƥ������~���i���\�঳�ᥢ���ɦV, ���D�A�b�C�@�B���B�z����.
>
> 3. ���A�Q�ϥ�`currentProfile`������, �A�����b���h�^�I���ʸ˨��޿�, �L�׬O�������覡�٬O�ϥΤ@�ӳ�W���������.
>
> Promises�ѨM�F�o�ǰ��D. �b�ڭ̶i�J���O�p��ѨM�o�ǰ��D���e, �����ڭ̨Ӭݬݤ@�Өϥ�promise��P�@���D����{.

	var currentProfile = fetchServerConfig().then(function(serverConfig){
		return fetchUserProfiles(serverConfig.USER_PROFILES, username);
	}).then(function{
		return profiles.currentProfile;
	}, function(error){
		// Handle errors in either fetchServerConfig or
		// fetchUserProfile here
	});

> �`�N���u��:
>
> 1. �A�i�H�챵��ƩI�s, �]���A���|�����Y�i�a�Ӫ�����.
>
> 2. �A�i�H��߫e�@�Ө�ƩI�s�|�b�U�@�Ө�ƩI�s���e����.
>
> 3. �C�@��`then()`�I�s���n��ӰѼ�(�o��ӰѼƳ��O���). �Ĥ@�ӰѼƬO���\���ާ@���^�I���, �ĤG�ӰѼƬO���~�B�z�����.
> 4. �b�챵���o�Ϳ��~�����p�U, ���~�T���|�g�ѿ��~�B�z���Ǽ������ε{������L����. �]��, ����^�I��ƪ����~���i�H�b�����Q�B�z.
>
> �A�|��, ������O`resolve`�M`reject`�O? �O��, `deferred`�bAngularJS���O�@�ثإ�promises���覡. �I�s`resolve`�Ӻ���promise(�I�s���\�ɪ��B�z���), �P�ɩI�s`reject`�ӳB�zpromise�b�I�s���~�B�z���ɪ��Ʊ�.

��ڭ��챵����Ѯ�, �ڭ̷|�A���^��o��.

###���O

�ڭ̲{�b�i�H�ಾ��Y�N�Φb�ڭ����ε{�������O�W��. �b�o�����ε{�����N����ӫ��O:

`butterbar`

�o�ӫ��O�N�b���ѵo�ͧ��ܨåB�������M�٦b�[���T���ɳB�z��ܩM���å���. ���N�s�������ܤƾ���, ��󭶭������A�Ӧ۰ʱ�����ܩΪ����ìO�_�ϥέ��Ӽ���.

`focus`

�o��`focus`���O�Ω�T�O���w����r��(�Ϊ̤���)�֦��J�I.

���ڭ̨Ӭݤ@�U�N�X:

	// This file is app/scripts/directives/directives.js

	var directive = angular.module('guthub.directives', []);

	directives.directive('butterbar', ['$rootScope', function($rootScope){
		return {
			link: function(scope, element attrs){
				element.addClass('hide');

				$rootScope.$on('$routeChangeStart', function(){
					element.removeClass('hide');
				});

				$routeScope.$on('$routeChangeSuccess', function(){
					element.addClass('hide');
				});
			}
		};
	}]);

	directives.dirctive('focus',function(){
		return {
			link: function(scope, element, attrs){
				element[0].focus();
			}
		};
	});

�W���ҭz�����O��^�@�ӹﹳ�a���@�ӳ�@���ݩ�, link. �ڭ̱N�b�Ĥ����`�J�Q�קA�i�H�p��إߧA�ۤv�����O, ���O�{�b, �A���Ӫ��D�U�����Ҧ��Ʊ�:

1. ���O�g�Ѩ�ӨB�J�B�z. �b�Ĥ@�B��(�sĶ���q), �Ҧ������O���Q���[��@�ӳQ�d��쪺DOM�����W, �M��B�z��. ����DOM�ާ@�_�o�ͦb�sĶ���q(�B�J��). �b�o�Ӷ��q������, ���ͤ@�ӳs�����.

2. �b�ĤG�B��, �s�����q(�ڭ̤��e�ϥΪ����q), ���ͫe����DOM�˪O�ós����@�ΰ�. �P�˪�, �����[��̩Ϊ̺�ť�����n�ھڻݭn�K�[, �b�@�ΰ�M�������e��^�@�Ӭ���(���V)�j�w. �]��, �������p��@�ΰ쪺�Ʊ����o�ͦb�s�����q.

����b�ڭ̫��O���o�ͤF����O? ���ڭ̥h�ݤ@��, �n��?

`butterbar`���O�i�H���U���o�˨ϥ�:

	<div butterbar>My loading text...</div>

�����e�����ê�����, �M��K�[��Ӻ�ť����ڧ@�ΰ줤. ��C���@�Ӹ��Ѷ}�l���ܮ�, ���N��ܸӤ���(�g�ѧ��ܥ���class[className]), �C�����Ѧ��\���ܨç�����, ���A�@������`butterbar`.

�t�@�Ӧ��쪺�Ʊ��O�`�N�ڭ̬O�p��`�J`$rootScopr`����O����. �Ҧ������O������������AngularJS���̿�`�J�t��, �]���A�i�H�`�J�A���A�ȩM��L����ݭn���F���䤤.

�̫�ݭn�`�N���O�B�z������API. �ϥ�jQuery���H�|�ܰ���, �]���L����ϥΪ��O�@������jQuery���y�k(addClass, removeClass). AngularJS��{�F�@�өI�sjQuery���ۤv, �]��, ������AngularJS���بӻ�, jQuery���O�@�ӥi�諸�̿ඵ. �p�G�A�̲צb�A�����ؤ��ϥΧ��㪺jQuery�w, �A���Ӫ��쥦�ϥΪ��O���ۤv���m��jQlite��{.

�ĤG�ӫ��O(focus)²��o�h. ���u�O�b��e�����W�I�s`focus()`��k. �A�i�H�ιL�b����input�����W�K�[`focus`�ݩʨөI�s��, �N���o��:

	<input type="text" focus></input>

�����[����, �����N�ߧY��o�J�I.

###���

�H�۫��O�M�A�Ȫ��л\, �ڭ̲ש�i�H�i�J��������F, �ڭ̦����ӱ��. �Ҧ����o�Ǳ�����b�@�ӳ�W�����(`app/scripts/controllers/controllers.js`), ���O�ڭ̷|�@�ӭӨ��A�ѥ���. ���ڭ̨ӬݲĤ@�ӱ��, �o�O�@�ӦC���, �t�d��ܨt�Τ��Ҧ������ЦC��.

	app.controller('ListCtrl', ['scope', 'recipes', function($scope, recipes){
		$scope.recipes = recipes;
	}]);

�`�N�C������̭��n���@�ӨƱ�: �b�o�ӱ����, ���èS���s������A���M���o�O����. �ۤ�, ���u�O�ϥΤw�g���o�����ЦC��. �A�i�ण���D���O�p��u�@��. �A�i��|�ϥθ��Ѥ@�`�Ӧ^��, �]�������@�ӧڭ̤��e�ݨ�`MultiRecipeLoader`. �A�u�ݭn�b�����̰O��.

�b�ڭ̴��쪺�C����U, ��L��������P���D�`�ۦ�, ���ڭ̤��M�|�v�B���X���̦��쪺�a��:

	app.controller('ViewCtrl', ['$scope', '$location', 'recipe', function($scope, $location, recipe){
			$scope.recipe = recipe;

			$scope.edit = function(){
				$location.path('/edit/' + recipe.id);
			};
	}]);

�o�ӵ��ϱ�������쪺�����O��s���Ƥ��}�b�@�ΰ줤. �Ӥ��O��ܩM���ær�q�Ϊ̨�L�������F��, �o�ӱ���̿��AngularJS�ӳB�z�c��������(�A���ӳo��)! �o�ӽs����²�檺����URL�ø����s�譹�Ъ�����, �A�i�H�ݨ�, AngularJS�èS���B�z�ѤU���u�@. AngularJS�ѧO�w�g���ܪ�URL�å[���^��������(�o�O�P�ڭ̽s��Ҧ����ۦP�����г���). �Ӭݤ@��!

���U��, ���ڭ̨Ӭݬݽs�豱�:

	app.controller('EditCtrl', ['$scope', '$location', 'recipe', function($scope, $location, recipe){
		$scope.recipe = recipe;

		$scope.save = function(){
			$scope.recipe.$save(function(recipe){
				$location.path('/view/' + recipe.id);
			});
		};

		$scope.remove = function(){
			delete $scope.recipe;
			$location.path('/');
		};
	}]);

����b�o�Ӽ��S�b�@�ΰ줤���s�豱����s��`save`�M`remove`��k������.

����A�Ʊ�@�ΰ줺��`save`��ư�����. ���O�s��e����, �åB�@���O�s�n, ���N�b�ù����N�Τ᭫�w�V��ۦP������. �^�I��ƬO�D�`���Ϊ�, �@���A�������Ȫ����p�U����Ϊ̳B�z�@�Ǧ欰.

����ؤ覡�i�H�b�o�̫O�s����. �@�جO�p�N�X�ҥ�, �g�Ѱ���$scope.recipe.$save()��k. �o�u�O�i��, �]��`recipe`�O�@�Ӹg�Ѷ}�Y������RecipeLoader��^���귽�ﹳ.

�t�~, �A�i�H���o�˨ӫO�s����:

	Recipe.save(recipe);

`remove`��Ƥ]�O��²�檺, �b�o�̥��|�q�@�ΰ줤��������, �P�ɱN�Τ᭫�w�V��D��歶. �Ъ`�N, ���èS���u�����q�ڭ̪����A���W�R����, ���ޥ��ܦA���X�B�~���I�s.

���U��, �ڭ̨Ӭݬ�New���:

	app.controller('NewCtrl', ['$scope', '$location', 'Recipe', function($scope, $location, Recipe){
		$scope.recipe = new Recipe({
			ingredents: [{}]
		});

		$scope.save = function(){
			$scope.recipe.$save(function(recipe){
				$location.path('/view/' + recipe.id);
			});
		};
	}]);

New����X�G�PEdit��������@��. ��ڤW, �A�i�H���X��ӱ���@���@�ӳ�@������Ӱ��@�ӽm��. �ߤ@���D�n���P�ONew����|�b�Ĥ@�B�إߤ@�ӷs������(�o�]�O�@�Ӹ귽, �]�����]���@��`save`���).��L���@�����O������.

�̫�, �ڭ��٦��@��Ingredients���. �o�O�@�ӯS�����, �b�ڭ̲`�J�A�ѥ�������Ϊ̦p��S���e, ���Ӭݤ@�ݥ�:

	app.controller('Ingredients', ['$scope', function($scope){
		$scope.addIngredients = function(){
			var ingredients = $scope.recipe.ingredients;
			ingredients[ingredients.length] = {};
		};

		$scope.removeIngredient = function(index) {
			$scope.recipe.ingredients.splice(index, 1);
		};
	}]);

��ثe����, �ڭ̬ݨ쪺�Ҧ���L����泽UI���ϤW�����������pô��. ���O�o��Ingredients����O�S��. ���O�@�Ӥl���, �Ω�b�s�譶���ʸ˯S�w�����ߦӤ��ݭn�b�~�h(����)�ӳB�z. ���쪺�O�n�`�N, �ѩ󥦬O�@�Ӧr���, �~�Ӧۧ@�ΰ줤�������(�b�o�̴N�OEdit/New���). �]��, ���i�H�X�ݨӦۤ������`$scope.recipe`.

�o�ӱ�������èS�����򦳽�Ϊ̿W�S���a��. ���u�O�K�[�@�ӷs��������{�������Ц����Ʋդ�, �Ϊ̱q���Ъ������C���R���@�ӯS�w������.

����{�b, �ڭ̴N�ӧ����̫᪺���. �ߤ@��JavaScript�N�X���i�ܤF�p��]�w����:

	// This file is app/scripts/controllers/controllers.js

	var app = angular.module('guthub', ['guthub.directives', 'guthub.services']);

	app.config(['$routeProvider', function($routeProvider){
		$routeProvider.
			when('/', {
				controller: 'ListCtrl',
				resolve: {
					recipes: function(MultiRecipeLoader) {
						return MultiRecipeLoader();
					}
				},
				templateUrl: '/views/list.html'
			}).when('/edit/:recipeId', {
				controller: 'EditCtrl',
				resolve: {
					recipe: function(RecipeLoader){
						return RecipeLoader();
					}
				},
				templateUrl: '/views/recipeForm.html'
			}).when('/view/:recipeId', {
				controller: 'ViewCtrl',
				resolve: {
					recipe: function(RecipeLoader){
						return RecipeLoader();
					}
				},
				templateUrl: '/views/viewRecipe.html'
			}).when('/new', {
					controller: 'NewCtrl',
					templateUrl: '/views/recipeForm.html'
			}).otherwise({redirectTo: '/'});
	}]);

���p�ڭ̩ҩӿժ�, �ڭ̲ש���A�ѪR��ƨϥΪ��a��. �e�����N�X�]�wGuthub AngularJS�Ҳ�, ���ѥH�ΰѻP���ε{�����˪O.

��������ڭ̤w�g�إߪ����O�M�A�ȤW, �M����w���P�����ѫ��V���ε{�������P�a��.

���C�Ӹ���, �ڭ̫��w�FURL, ���ƥ����, �[���˪O, �H�γ̫�(�i�諸)���ѤF�@��`resolve`�ﹳ.

�o��`resolve`�ﹳ�|�i�DAngularJS, �C��resolve��ݭn�b�T�w���ѥ��T�ɤ~����ܵ��Τ�. ��ڭ̨ӻ�, �ڭ̷Q�n�[���Ҧ������ЩΪ̭ӧO���t��, �ýT�O�b��ܭ������e���A���n�^���ڭ�. �]��, �ڭ̭n�i�D���Ѵ��Ѫ̧ڭ̪�����, �M��A�i�D�L�p��Ө��o��.

�o�����`���ڭ̦b�Ĥ@�`���w�q�F��ӪA��, ���O��`MultiRecipeLoader`�M`RecipeLoader`. �p�G`resolve`��ƪ�^�@��AngularJS promise, �M��AngularJS�|����b��o�����e����promise�ѨM���D. �o�N���ۥ��N�|���ݨ���A���^��.

�M��N��^���G�ǻ���c�y��Ƥ��@���Ѽ�(�P�Ӧ۹ﹳ�r�q���Ѽƪ��W�٤@�_�@���Ѽ�).

�̫�, `otherwise`��ƪ�ܷ�S�����Ѥǰt�ɭ��w�V���q�{URL.

> �A�i��|�`�N��Edit�MNew�����Ӹ��ѳq�V�P�@�Ӽ˪OURL, `views/recipeForm.html`. �o�̵o�ͤF����O? �ڭ̴_�ΤF�s��˪O. �̿����������, �N���P��������ܦb�s�譹�м˪O��.

�����o�Ǥu�@����, �{�b�ڭ̥i�H�E�J��˪O����, �Ӭݬݱ���p�󱾱��쥦�̤��W, �H�Φp��޲z�{�굹�̲ץΤ᪺���e.

##�˪O

���ڭ̭����Ӭݬݳ̥~�h���D�˪O, �o�̴N�O`index.html`. �o�O�ڭ̳歶���ε{������¦, �P�ɩҦ���L�����Ϥ]�|�˦b��o�Ӽ˪O���W�U�夤:

	<!DOCTYPE html>
	<html lang="en" ng-app="guthub">
	<head>
		<title>Guthub - Create and Share</title>
		<script src="scripts/vendor/angular.min.js"></script>
		<script src="scripts/vendor/angular-resource.min.js"></script>
		<script src="scripts/directives/directives.js"></script>
		<script src="scripts/services/services.js"></script>
		<script src="scripts/controlers/controllers.js"></script>
		<link rel="stylesheet" href="styles/bootstrap.css">
		<link rel="stylesheet" href="styles/guthub.css">
	</head>
	<body>
		<header>
			<h1>Guthub</h1>
		</header>
		<div butterbar>Loading...</div>

		<div class="container-fluid">
			<div class="row-fluid">
				<div class="span2">
					<!-- Sidebar -->
					<div class="focus"><a href="/#/new">New Recipe</a></div>
					<div><a href="/#/">Recipe List</a></div>
				</div>
				<div class="span10">
					<div ng-view></div>
				</div>
			</div>
		</div>
	</body>
	</html>

�`�N�e�����˪O����5�Ӧ��쪺����, �䤤�j�����A�b��2�������w�g���L�F. ���ڭ̳v�ӨӬݬݥ���:

`ng-app`

�ڭ̳]�w�F`ng-app`�Ҳլ�Guthub. �o�P�ڭ̦b`angular.module`��Ƥ����Ѫ��ҲզW�٬ۦP. �o�K�OAngularJS�p�󪾹D��ӱ����b�@�_����].

`script`����

�o������ε{���b���̥[��AngularJS. �o�����b�Ҧ��ϥ�AngularJS��JS���Q�[�����e����. �z�Q�����p�U, �����Ӧbbody����������(\</body\>���e).

`Butterbar`

�ڭ̲Ĥ@���ϥΦ۩w�q���O. �b�ڭ̩w�q�ڭ̪�`butterbar`���O���e, �ڭ̧Ʊ�N���Ω�@�Ӥ���, �H�K�b���ѧ��ܮ���ܥ�, �b���\���ɭ����å�(loading...�B�z). �ݭn��X��ܳo�Ӥ�������r(�b�o�̧ڭ̨ϥΤF�@�ӫD�`�ФH��"Loading...").

�챵��`href`��

`href`�Ω��챵��ڭ̳歶���ε{�����U�ӭ���. �l���̦p��ϥ�#�r�ŨӽT�O�������|������, �åB�۹���e����. AngularJS�|�ʱ�URL(�u�n�����S������), �M��b�ݭn���ɭ԰_�쯫�_���@��(�Ϊ̳q�`, �N�o�ӫD�`�ФH�����Ѻ޲z�w�q���ڭ̸��Ѫ��@����).

`ng-view`

�o�O�̫�@�ӯ��_���ǧ@. �b�ڭ̪�����@�`, �ڭ̩w�q�F����. �@���w�q���@����, �C�Ӹ��Ѫ�ܤ@��URL, ������p���ѩM�@�Ӽ˪O. ��AngularJS�o�{�@�Ӹ��ѧ��ܮ�, ���N�|�[�����p���˪O, �ñN����K�[����, �P�ɴ���`ng-view`���Ӽ˪O�����e.

���@��ޤH�`�ت��Ʊ��O�o�̯ʤ�`ng-controller`����. �j�������ε{���Y�ص{�פW���ݭn�@�ӻP�~���˪O���p��MainController. ��̱`������m�O�bbody���ҤW. �b�o�ر��p�U, �ڭ̨èS���ϥΥ�, �]�����㪺�~���˪O�S��AngularJS���e�ݭn�ޥΨ�@�ӧ@�ΰ�.

�{�b�ڭ̨ӬݬݻP�C�ӱ�����p����W���˪O, �N�q"���ЦC��"�˪O�}�l:

	<!-- File is chapter4/guthub/app/view/list.html -->
	<h3>Recipe List</h3>
	<ul class="recipes">
		<li ng-repeat="recipe in recipes">
			<div><a ng-href="/#/view/{{recipe.id}}">{{recipe.title}}</a></div>
		</li>
	</ul>

�O��, ���O�@�ӫD�`�L��(���q)���˪O. �o�̥u����Ӧ��쪺�I. �Ĥ@�ӬO�D�`�зǪ�`ng-repeat`���ҥΪk. �L�|��o�@�ΰ줺���Ҧ����Шí����˥X����.

�ĤG�ӬO`ng-href`���Ҫ��Ϊk�Ӥ��O`href`�ݩ�. �o�O�@�ӦbAngularJS�[�������º�L�Ī��ť��챵. `ng-href`�|�T�O����ɭԳ����|���Τ�e�{�@�ӷ�Ϊ��챵. �`�O�|�ϥΥ��b����ɭԨϧA��URLs���O�ʺA���Ӥ��O�R�A��.

��M, �A�i��P��_��: ����b����? �o�̨S��`ng-controller`�w�q, �]�T��S��Main Controller�w�q. �o�O���ѬM�g�o�����@��. �p�G�A�ٰO�o(�Ϊ̩��e½�X��), `/`���ѷ|���w�V��C��˪O�åB�a���P�����p��ListController. �]��, ��ޥΥ����ܼƩΪ��������F���, �����bList Controller�@�ΰ줺��.

�{�b�ڭ̨Ӭݤ@�Ǧ���h��褺�e���F��: ���ϧΦ�.

	<!-- File is chapter4/guthub/app/views/viewRecipe.html -->
	<h2>{{recipe.title}}</h2>

	<div>{{recipe.decription}}</div>

	<h3>Ingredients</h3>
	<span ng-show="recipe.ingredients.length == 0">No Ingredients</span>
	<ul class="unstyled" ng-hide="recipe.ingredients.length == 0">
		<li ng-repeat="ingredient in recipe.ingredients">
			<span>{{ingredient.amount}}</span>
			<span>{{ingredient.amountUnits</span>
			<span>{{ingredient.ingredientName}}</span>
		</li>
	</ul>

	<h3>Instructions</h3>
	<div>{{recipe.instructions}}</div>

	<form ng-submit="edit()" class="form-horizontal">
		<div class="form-actions">
			<button class="btn btn-primary">Edit</button>
		</div>
	</form>

�o�O�t�@�Ӥ�����, �ܤp���]�t�˪O. �ڭ̱N�����A�`�N�T���, ���M���|���ӥ��̩ҥX�{������.

�Ĥ@�ӴN�O�D�`�зǪ�`ng-repeat`. ����(recipes)�A���X�{�bView Controller�@�ΰ줤, �o�O�ιL�b�����{�굹�Τᤧ�e�g��`resolve`��ƥ[����. �o�T�O�Τ�d�ݥ��ɤ]�����O�@�ӯ}�H��, ���[�������A.

���U�Ӥ@�Ӧ��쪺�Ϊk�O�ϥ�`ng-show`�M`ng-class`(�o�����ӬO`ng-hide`)�ӳ]�w�˪O���˦�. `ng-show`���ҳQ�K�[��\<i\>���ҤW, �o�O�Ψ���ܤ@�ӬP���аO��icon. �{�b, �o�ӬP���аO�u�b���ЬO�@�ӯS�⭹�Ъ��ɭԤ~���(�Ҧp�g��`recipe.featured`�����ȨӼаO). �z�Q�����p�U, ���F�T�O�A�����Z, �A�ݭn�ϥΤ@�Ӫťժ��Ů�ϼ�, �õ��o�ӪŮ�ϼиj�w`ng-hide`���O, �M��P�k�P�˪�AngularJS��F��`ng-show`�����. �o�O�@�ӱ`�����Ϊk, ��ܤ@�ӪF��æb���w������U������.

`ng-class`�Ω�K�[�@����(CSS��)��\<h2\>����(�b�o�ر��p�U�N�O"�S��")���ЬO�@�ӯS�⭹�Ю�. ���K�[�F�@�ǯS�����G�Өϼ��D��[�ޤH�`��.

�̫�@�ӻݭn�`�N���ɪ��W��`ng-submit`���O. �o�ӫ��O�W�w�b���Q���檺���p�U�I�s`scope`����`edit()`���. �����S�����p���T��ƪ����s�Q�I���ɾ��|������(�o�ر��p�U�K�OEdit���s). �P��, AngularJS�������઺�b�@�ΰ줤(�q�Ҳ�,����,�����)�b���T���ɶ��̤ޥΩM�I�s���T����k.

> **�W���o�q�����P��ѥN�X���@�Ǯt�O, Ū�̦ۦ�z��. ��ѧ@�̼ȥ����X�ѵ�.**

�{�b�ڭ̥i�H�Ӭݬݧڭ̳̫᪺�˪O(�i��ثe����̽������@��), ���Ъ��˪O:

	<!-- file is chapter4/guthub/app/views/recipeForm.html -->
	<h2>Edit Recipe</h2>
	<form name="recipeForm" ng-submit="save()" class="form-horizontal">
		<div class="control-group">
			<label class="control-label" for="title">Title:</label>
			<div class="controls">
				<input ng-model="recipe.title" class="input-xlarge" id="title" focus required>
			</div>
		</div>

		<div class="control-group">
			<label class="control-label" for="description">Description:</label>
			<div class="controls">
				<textarea ng-model="recipe.description" class="input-xlarge" id="description"></textarea>
			</div>
		</div>

		<div class="control-group">
			<label class="control-label" for="ingredients">Ingredients:</label>
			<div class="controls">
				<ul id="ingredients" class="unstyled" ng-controller="IngredientsCtrl">
				<li ng-repeat="ingredient in recipe.ingredients">
					<input ng-model="ingredient.amount" class="input-mini">
					<input ng-model="ingredient.amountUnits" class="input-small">
					<input ng-model="ingredient.ingredientName">
					<button type="button" class="btn btn-mini" ng-click="removeIngredient($index)"><i class="icon-minus-sign"></i> Delete </button>
				</li>
				<button type="button" class="btn btn-mini" ng-click="addIngredient()"><i class="icon-plus-sign"></i> Add </button>
			</ul>
			</div>
		</div>

		<div class="control-group">
			<label class="control-label" for="instructions">Instructions:</label>
			<div class="controls">
				<textarea ng-model="recipe.instructions" class="input-xxlarge" id="instructions"></textarea>
			</div>
		</div>

		<div class="form-actions">
			<button class="btn btn-primary" ng-disabled="recipeForm.$invalid">Save</button>
			<button type="button" ng-click="remove()" ng-show="!recipe.id" class="btn">Delete</button>
		</div>
	</form>

���n��W. ���ݰ_�ӹ��ܦh�N�X, �åB���ɤ@�ӫܪ����N�X, ���O�p�G�A�{�u��s�H�U��, �A�|�o�{���ä��O�D�`����. �ƹ�W, �䤤�ܦh���O��²�檺, ��p���ƪ���ܥi�s���J�r�q�Ω�s�譹�Ъ��˪O:

+ `focus`���O�Q�K�[��Ĥ@�ӿ�J�r�q�W(`title`��J�r�q). �o�T�O��Τ�ɯ��o�ӭ�����, ���D�r�q�|�۰ʻE�J, �åB�Τ�i�H�ߧY�}�l��J���D�T��.

+ `ng-submit`���O�P�e�����Ҥl�D�`�ۦ�, �]���ڭ̤��|�`�J�Q�ץ�, ���u�O�O�s�O���Ъ����A�M�s��L�{�������H��. ���|������Edit Controller����`save()`���.

+ `ng-model`���O�Ω�N���P����r��J�ةM��r��j�w��ҫ���.

�b�o�ӭ����󦳽쪺�@�譱, �åB�ڭ̫�ĳ�A��@�I�������A�ѥ����K�O�t�ƦC������`ng-controller`����. ���ڭ̪�@�������ƥ���A�ѥH�U�o�̵o�ͤF����.

�ڭ̬ݨ�F�@����ܰt�Ʀ������C��, �åB�e���������p�F�@��`ng-controller`. �o�N���۳o��`\<ul\>`���ҬOIngredients Controller���@�ΰ�. ���O�o�Ӽ˪O��ڪ�����O����O, �OEdit Controller? �ƹ��ҩ�, Ingredients Controller�O�@��Edit Controller���l����إߪ�, �q���~�ӤFEdit Controller���@�ΰ�. �o�N�O�����򥦥i�H�qEdit Controller�X�ݭ��йﹳ(recipe object)����].

���~, ���ټW�[�F�@��`addIngredient()`��k, �o�O�g�ѳB�z���G��`ng-click`�ϥΪ�, ����N�u��b`\<ul\>`���ҧ@�ΰ줺�X��. ���򬰤���A�ݭn�o�򰵩O? �]���o�O�����A��~���̦n���覡. ������Edit Controller�ݭn�@��`addIngredients()`��k, ��99%���˪O�����|���ߥ�. �]���p����T�A���l����M�O�M����O�ܤ�����, ���i�H�]�t���Ȩô`�ǧA�����A���~���޿���h���i���@�Ҳդ�.

+ �t�~�@�ӱ���K�O�ڭ̦b�o�̷Q�n�`�J�Q�ת�������ұ���. ���ܮe���bAngularJS���]�w�@�ӯS�w�����r�q��"����". �u�ݭn²�檺�K�[required���Ҩ��J�ؤW(�P�e�����N�X�������p�@��). ���O�{�b�A�n���復.

����, �ڭ̥�����O�s���s����. �`�N���W�����@��`ng-disabled`���O, �o�������N�O`recipeForm.$invalid`. �o��`recipeForm`�O�ڭ̤w�g�n�������W��. AngularJS�W�[�F�@�ǯS���ܼ�(`$valid`�M`$invalid`�u�O�䤤���)���\�A�����檺����. AngularJS�|�d���Ҧ������񤸯��ç�s�ҹ������S���ܼ�. �]���p�G�ڭ̪�Recipe Title����, `recipeForm.$invalid`�N�|�Q�o�u��true(`$valid`�N��false), �P�ɧڭ̪��O�s(Save)���s�N�|�ߨ�Q�T��.

�ڭ��٥i�H���@�Ӥ�r��J�س]�w�̤j�M�̤p����(��J����), �H�Τ@�ӥΩ����Ҥ@�ӿ�J�r�q�����h��F���Ҧ�. �t�~, �o���٦��u�b�����S�w����ɥΩ���ܯS�w���~�������i���Ϊk. ���ڭ̨ϥΤ@�ӫܤp������Ҥl�Ӭݬ�:

	<form name="myForm">
		User name: <input type="text" name="userName" ng-model="user.name" ng-minlength="3">
		<span class="error" ng-show="myForm.userName.$error.minlength">Too Short!</span>
	</form>

�b�e�����o�ӨҤl��, �ڭ̲K�[�F�@�n�D: �Τ�W�ܤ֬O�T�Ӧr��(�g�Ѩϥ�`ng-minlength`���O). �{�b, ���d�򤺷|���ߨC�өR�W��J�ت���R�Φ�--�b�o�ӨҤl���ڭ̥u���@��`userName`--�䤤�C�ӿ�J�س��|���@��`$error`�ﹳ(�o�̨��骺�٥]�A����˪����~�Ϊ̨S�����~: `required`, `minlength`, `maclength`�Ϊ̼Ҧ�)�M�@��`$valid`���ҨӪ�ܿ�J�إ����O�_����.

�ڭ̥i�H�Q�γo�Өӿ�ܩʪ��N���~�T����ܵ��Τ�, �o�ھڤ��Ϊ���J���~���������, ���p�ڭ̤W������ҩҥ�.

���^��ڭ̭�Ӫ��˪O��--Recipe���˪O--�b�o�̪�ingredients repeater�̭��٦��t�~�@�ӫܦn��`ng-show`���G���Ϊk. �o��Add Ingredient���s�u�|�b�̫᪺�@�Ӱt�ƪ��������. �ۥi�H�g�Ѧb�@��repeater�����d�򤺩I�s�@��`ng-show`�èϥίS��`$last`�ܼƨӧ���.

�̫�ڭ��٦��̫᪺�@��`ng-click`, �o�O���[���ĤG�ӫ��s, �Ω�R���ӭ���. �`�N�o�ӫ��s�u�|�b���Щ|���O�s���ɭ����. ���M�q�`���|�s�g�@�ӧ󦳷N�q��`ng-hide="recipe.id", ���ɭԥ��|�ϥΧ󦳻y�q��`ng-show="!recipe.id". �]�N�O��, �p�G���ШS���@��id���ɭ����, �Ӥ��O�b���Ц��@��id���ɭ�����.

##����

�H�۱������, �ڭ̤w�g����V�A��ܴ��ճ����F, ���A���D���|�Y�N���, ���O��? �b�o�@�`, �ڭ̱N�|�[�\�A�w�g�s�g�������N�X����, �H�ίA�ΧA�n�p��s�g����.

###�椸����

�Ĥ@��, �]�O�D�`���n���@�ش��լO�椸����. ��󱱨(���O�M�A��)�����էA�w�g�}�o�M�s�g�����T�����c, �åB�A�i��|�Q�쥦�̷|������.

�b�ڭ̲`�J��U�ӳ椸���դ��e, ���ڭ̳�¶�Ҧ��ڭ̪�����椸���ըӬݬݴ��ո˸m:

	describle('Controllers', function() {
		var $scope, ctrl;
		//you need to include your module in a test
		beforeEach(module('guthub'));
		beforeEach(function() {
			this.addMatchers({
				toEqualData: function(expected) {
					return angular.equals(this.actual, expected);
				}
			});
		});

		describle('ListCtrl', function() {....});
		// Other controller describles here as well
	});

�o�Ӵ��ո˸m(�ڭ̤��M�ϥ�Jasmine���欰�覡�ӽs�g�o�Ǵ���)���F�X��Ʊ�:

1. �إߤ@�ӥ���(�ܤֹ��o�Ӵ��ճW�d�O�o�ӥت�)�i�X�ݪ��@�ΰ�M���, �ҥH�ڭ̤��ξ�ߨC�ӱ���|�إߤ@�ӷs���ܼ�.

2. ��l�Ƨڭ����ε{���ҥΪ��Ҳ�(�b�o�̬OGuthub).

3. �K�[�@�ӧڭ̺٤���`equalData`���S���ǰt��. �o�򥻤W���\�ڭ̦b�귽�ﹳ(�N������)�g��`$resource`�A�ȩM�I�sRESTful�Ӱ����_��(���էP�_).

> �O�o�b����ڭ̳B�z�b`ngRsource`�W��^��H���_���ɲK�[�@�Ӻ٬�`equalData`�S��ǰt��. �o�O�]��`ngRsource`��^�ﹳ�٦��B�~����k�b���̥��Ѯ��q�{�Ʊ�I�sequal��k.

�o�Ӹ˸m�즹����, ���ڭ̨Ӭݬ�List Controller���椸����:

	describle('ListCtrl', function(){
		var mockBackend, recipe;
		// _$httpBackend_ is the same as $httpBackend. Only written this way to diiferentiate between injected variables and local variables
		breforeEach(inject(function($rootScope, $controller, _$httpBackend_, Recipe) {
			recipe = Recipe;
			mockBackend = _$httpBackend_;
			$scope = $rootScope.$new();
			ctrl = $controller('ListCtrl', {
				$scope: $scope,
				recipes: [1, 2, 3]
			});
		}));

		it('should have list of recipes', function() {
			expect($scope.recipes).toEqual([1, 2, 3]);
		});
	});

�O��o��List Controller�u�O�ڭ̳�²�檺������@. �o�ӱ�����c�y���u�O�����@�ӭ��ЦC��ñN���O�s��@�ΰ줤. �A�i�H�s�g�@�Ӵ��յ���, �������G���@�I���X�z(�ڭ��٬O�o�򰵤F, �]���o�Ӵ��իܤ���).

�ۤ�, �󦳽쪺�OMulyiRecipeLoader�A�Ȥ譱. ���t�d�q���A���W���o���ЦC��ñN���@���@�ӰѼƶǻ�(��g��`$route`�A�ȥ��T���s����).

	describe('MultiRecipeLoader', function() {
		var mockBackend, recipe, loader;
		// _$httpBackend_ is the same as $httpBackend. Only written this way to differentiate between injected variables and local variables. 

		beforeEach(inject(function(_$httpBackend_, Recipe, MultiRecipeLoader) {
			recipe = Recipe;
			mockBackend = _$httpBackend_;
			loader = MultiRecipeLoader;
		}));

		it('should load list of recipes', function() { 
			mockBackend.expectGET('/recipes').respond([{id: 1}, {id: 2}]);

			var recipes;

			var promise = loader(); promise.then(function(rec) {
				recipes = rec;
			});

			expect(recipes).toBeUndefined( ) ;

			mockBackend. f lush() ;

			expect(recipes).toEqualData([{id: 1}, {id: 2}]); });
	});
	// Other controller describes here as well

�b�ڭ̪����դ�, �ڭ̸g�ѱ�����@�Ӽ�����`HttpBackend`�Ӵ���MultiRecipeLoader. �o�Ӧ۩���չB��ɩҥ]�t��`angular-mocks.js`���. �u�ݱN���`�J��A��`beforeEach`��k���N���H���A�]�w�w���ت�. ���U��, �ڭ̶i��F�@�ӧ󦳷N�q������, �ڭ̴���]�w�@�Ӧ��A����GET�ШD�Ө��orecipes, ������^�@��²�檺�Ʋչﹳ. �M��ϥΧڭ̷s���۩w�q���ǰt���ӽT�O���T����^���. �`�N�b����backend����`flush()`�I�s, �o�N�i�D����Backend�q���A����j�^��. �A�i�H�ϥγo�Ӿ���Ӵ��ձ���y�{�M�d�ݧA�����ε{���b���A����^�@�Ӧ^�����e�M����O�p��B�z��.

�ڭ̱N���LView Controller, �]�������F�b�@�ΰ줤�K�[�@��`edit()`��k���~���PList Controller�@�Ҥ@��. �o�O�D�`²�檺����, �A�i�H�b�A�����դ��`�J`$location`���ˬd������.

�{�b���ڭ̸���Edit Controller, �䤤����Ӧ��쪺�I�ڭ̶i��椸����. �@�ӬO�����ڭ̤��e�ݨ�L��`resolve`���, �åB�i�H�H�P�˪��覡����. �ۤ�, �ڭ̲{�b�Q�ݬݧڭ̥i�H�p�M����`save()`�M`remove()`��k. ���ڭ̨Ӭݬݹ�󥦭̪�����(���]�ڭ̪����դu��Ӧ۩�e�����Ҥl):

	describle('EditController', function() {
		var mockBackend, location;
		beforeEach(inject($rootScope, $controller, _$httpBackend_, $location, Recipe){
			mockBackend = _$httpBackend_;
			location = $location;
			$scope = $rootScope.$new();

			ctrl = $controller('EditCtrl', {
				$scope: $scope,
				$location: $location,
				recipe: new Recipe({id: 1, title: 'Recipe'});
			});
		}));

		it('should save the recipe', function(){
			mockBackend.expectPOST('/recipes/1', {id: 1, title: 'Recipe'}).respond({id: 2});

			// Set it to something else to ensure it is changed during the test
			location.path('test');

			$scope.save();
			expect(location.path()).toEqual('/test');

			mockBackend.flush();

			expect(location.path()).toEqual('/view/2');
		});

		it('should remove the recipe', function(){
			expect($scope.recipe).toBeTruthy();
			location.path('test');

			$scope.remove();

			expect($scope.recipe).toBeUndefined();
			expect(location.path()).toEqual('/');
		});
	});

�b�Ĥ@�Ӵ��ե�, �ڭ̴��դF`save()`���. �S�O�O, �ڭ̽T�O�b�ڭ̪���H�O�s�ɭ����إߤ@�Ө���A����POST�ШD, �M��, �@�����A���^��, �a�}�N���ܨ�s�����[��H�����ϭ��Э���.

�ĤG�Ӵ��է�²��. �ڭ̶i��F²�檺�˴��H�T�O�b�@�ΰ줤�I�s`remove()`��k���ɭԲ�����e����, �M�᭫�w�V��Τ�D��. �o�i�H�ܮe���g�Ѫ`�J`$location`�A�Ȩ�ڭ̪����դ��èϥΥ�.

��l���w�ﱱ����椸���տ�`�D�`�ۦ����Ҧ�, �]���b�o�̧ڭ̸��L����. �b�L�̪����h��, �o�ǳ椸���ը̿��@�ǨƱ�:

+ �T�O���(�Ϊ̧�i��O�@�ΰ�)�b������l�ƮɹF�쥿�T�����A

+ �T�{�g�楿�T�����A���I�s, �H�θg�ѧ@�ΰ�b���A���I�s�����M������h�����T�����A(�g�Ѧb�椸���դ��ϥΧڭ̪�������ݪA��)

+ �Q��AngularJS���̿�`�J�ج[�ۤ�B�z�����H�α���ﹳ�Ω�T�O����|�]�w���T�����A.

###�}������

�@���ڭ̹�椸���իܺ��N, �ڭ̥i��T��������a�@�U, ��ڳ��X, ���u. ���OAngularJS�}�o�̤��|�o��, ����L�̧����F�L�̪��}������(��������). ���M�椸���սT�O�ڭ̪��C�@��JS�N�X�����ӹw���u�@, �ڭ̤]�n�T�O�˪O�[��, �å��T�������챱��W, �H�Φb�˪O���I�������T���Ʊ�.

�o���OAngularJS�a���A���}������(��������), �����\�A���H�U�Ʊ�:

+ �[���A�����ε{��

+ �s���@�ӯS�w������

+ �H�N���I���P��M��J��r

+ �T�O�o�ͥ��T���Ʊ�

�ҥH, �}�����զp��b�ڭ̪�"���ЦC��"�����u�@? ����, �b�ڭ̶}�l��ڪ����դ��e, �ڭ̻ݭn���@�ǰ�¦�u�@.

���Ӹ}�����դu�@, �ڭ̻ݭn�@�Ӥu�@��Web���A���H�ǳƱqGuthub���ΤW�����ШD, �P�ɱN���\�ڭ̱q���W���s�x�M���o�@�ӭ��ЦC��. �H�N�����N�X�H�ϥΤ��s�������ЦC��(����`$resource`���Шåu�O�N���ഫ���@��JSON�ﹳ), �Ϊ̴_�ΩM�ק�ڭ̫e�����`�V�A�i�ܪ�Web���A��, �Ϊ̨ϥ�Yeoman!

�@���ڭ̦��F�@�Ӧ��A���ùB��_��, �P�ɪA�ȩ�ڭ̪����ε{��, �M��ڭ̴N�i�H�s�g�M�B��U��������:

	describle('Guthub App', function(){
		it('should show a list of recipes', function(){
			browser().navigateTo('/index.html');
			//Our Default Guthub recipes list has two recipes
			expect(repeater('.recipes li').count()).toEqual(2);
		});
	});
