#�P���A���q�H

��{�b����A�ڭ̤w�g�ݨ�U���o�Ǥ��e���D�n�����A�o�Ǥ��e�O�A��Angular���Φp��W���]�p�B���P��AngularJS����p��˰t�b�@�_�å��`�u�@�H��AngularJS�����˪O�N�X�B�����@�p�������e�C��o�ǵ��X�b�@�_�A�A�N�i�H�f�ؤ@�ǭ]���ʷP��Web���ΡA���L�̪��B�@�D�n�٬O����b�Ȥ��.�b�e���ĤG��,�ڭ̬ݤF�@�I��`$http`�A�Ȱ����A���ݳq�H�����e,���O�b�o�@��,�ڭ̱N�|�`�J���Q�@�U�p��b�{��@�ɪ����Τ��ϥΥ�(`$http`)

�b�o�@���A�ڭ̱N�Q�פ@�UAngularJS�p�����A�P���A���ݳq�H�A�o�䤤�]�A�b�̩��⹳���Ū��h���Ϊ̥Υ����Ѫ��u�����ʸ˾��C�ӥB�ڭ̱N�|�`�J���QAngularJS�p��Τ��ا֨���������A�[�t�A������.�p�G�A�Q��`SocketIO`�}�o�@�ӹ�ɪ�Angular����,����ĤK�����@�ӨҤl�A�t�ܤF�p���PSocketIO�P�ʸ˦��@�ӫ��O�M��p��ϥγo�ӫ��O�A�b�o�@���A�ڭ̴N���A�γo�譱���e�F.

##�g��$http�i��q��

�qAjax����(�ϥ�XMLHttpRequests)�o�ʤ@�ӽШD����A�����ǲΤ覡�]�A�G�o��@��XMLHttpRequest��H���ޥΡB�o�_�ШD�BŪ���^���B������~�N�X�M��̫�B�z���A���^���C���N�O�U���o�ˡG
    
    var xmlhttp = new XMLHttpRequest();
    xmlhttp.onreadystatechange = function() {
        if (xmlhttp.readystate == 4 && xmlhttp.status == 200) {
            var response = xmlhttp.responseText;
        } else if (xmlhttp.status == 400) { // or really anything in the 4 series
            // Handle error gracefully
        }
    };
    // Setup connection
    xmlhttp.open(�uGET�v, �uhttp://myserver/api�v, true);
    // Make the request
    xmlhttp.send();
    
���o�ˤ@��²��B�`�ΥB�g�`���ƪ����ȡA�W���o�ӥN�X�q����j.�p�G�A�Q���Ʃʦa���o���,�A�̲ץi��|���@�ӫʸ˩Ϊ̨ϥβ{�����禡�w.

AngularJS XHR(XMLHttpRequest) API��`Promise���f.�]��XHRs�O�D�P�B��k�I�s�A���A���^���N�|�b���Ӥ@�Ӥ��w���ɶ���^(��M�Ʊ�O�V�ֶV�n).Promise���f�O�ҤF�o�˪��^���N�|�p��B�z,�����\Promise���f�����O�̥H�@�إi�w�p���覡�ϥγo�Ǧ^��.

���]�ڭ̷Q�q�ڭ̪����A�����^�Τ᪺�T��.�p�G���f�b/api/user�a�}�i��,�åB����id�@��url�ѼơA����ڭ̪�XHR�ШD�N�i�H���U���o�˨ϥ�Angular���֤�$http�A��:
    
    $http.get('api/user', {params: {id: '5'}
    }).success(function(data, status, headers, config) {
    // Do something successful.
    }).error(function(data, status, headers, config) {
    // Handle the error
    });
    
�p�G�A�Ӧ�jQuery�@��,�A�i��|�`�N��GAngularJS�MjQuery�B�z�D�P�B�ݨD���覡�ܬۦ�.

�ڭ̤W���Ҥl���ϥΪ�$htttp.get��k�ȶȬOAngularJS�֤ߪA��$http���Ѫ����h²�K��k���@.�������A�p�G�A�Q�ϥ�AngularJS�V�ۦPURL�a�@��POST�ШD��Ƶo�_�@��POST�ШD�A�A�i�H���U���o�˰��G

    var postData = {text: 'long blob of text'};
    // The next line gets appended to the URL as params
    // so it would become a post request to /api/user?id=5 
    var config = {params: {id: '5'}};
    $http.post('api/user', postData, config
    ).success(function(data, status, headers, config) {
    // Do something successful
    }).error(function(data, status, headers, config) {
    // Handle the error
    });

AngularJS���j�h�Ʊ`�νШD���������ѤF������²�K��k�A�L�̥]�A�G

+ GET
+ HEAD
+ POST
+ DELETE
+ PUT
+ JSONP

###�i�@�B�t�m�A���ШD

���ɡA�u��c���Ѫ��зǽШD�t�m�٤���,���i��O�]���A�Q���U���o�ǨƱ�:

+ �A�i��Q���ШD�K�[�v�����Ҫ��Y�T��
+ ���ܽШD��ƪ��֨��覡
+ �b�ШD�Q�o�e�Ϊ̦^����^�ɡA���ƥH�@�Ǥ覡���@�w���ഫ�B�z

�b�W���o�˪����p���U,�A�i�H�i�@�B�t�m�ШD�A�g�ѥi�諸�ǻ��i�ШD���t�m�ﹳ.�b���e���Ҥl��,�ڭ̨ϥΰt�m�ﹳ�ӼЩ��i�諸URL�ѼơA�Y�K�ڭ̭���t�ܪ�GET�MPOST��k�O²�K��k�C��������ͤ�k�i��ݤW�����ۭ��o�ˡG

    $http(config)

�U���t�ܪ��O�@�өI�s�o�Ӥ�k�����N�X�˪O:

    $http({
        method: string,
        url: string,
        params: object,
        data: string or object,
        headers: object,
        transformRequest: function transform(data, headersGetter) or an array of functions,
        transformResponse: function transform(data, headersGetter) or an array of functions,
        cache: boolean or Cache object,
        timeout: number,
        withCredentials: boolean
    });

GET�BPOST�M�䥦��²�K��k�w�g�]�w�F�ШD��method����,�ҥH���ݭn�A�]�w�o�ӡAconfig�t�m��H�O�ǵ��P$http.get�P�B�P$http.post�P��k���̫�@�ӰѼ�,�ҥH��A�ϥΥ���²�K��k���ɭԡA�A�����γo��config�t�m�ﹳ.

�A�]�i�H�g�ѶǤJ�t���U���o���䪺�ݩʶ�config�ﹳ�ӧ��ܤw����request�ﹳ

+ method : �@�Ӫ��http�ШD�������r�Ŧ�A��pGET,�Ϊ�POST
+ url : �@��URL�r�Ŧ�N��n�ШD�귽������ά۹�URL
+ params : �@�ӹﹳ(�ǽT�����O��ȬM�g)�]�t�r�Ŧ��r�Ŧꤺ�e�A���N��F�N�|�ഫ��URL�Ѽƪ���ȹ�A��p�U���o�ˡG
    [{key1: 'value1', key2: 'value2'}]
���N�|�Q�ഫ��:
    ?key1=value&key2=value2
�o��r�űN�|�[�bURL�᭱�A�p�G�bvalue����m�A�Τ@�ӹﹳ���N�r�Ŧ�μƦr�A���o�ӹ�H�N�|�ഫ��JSON�r�Ŧ�.
+ data �G�@�Ӧr�Ŧ�Τ@�ӹ�H�A���N�|�Q�@���ШD������ƳQ�o�e.
+ timeout : �o�O�ШD�Q�{�w���L�����e�ҭn���ݪ��@���.

�٦������t�~���ﶵ�i�H�Q�t�m,�b�U�������`���A�ڭ̱N�|�`�ױ����o�ǿﶵ.

###�]�wHTTP�Y�T��(Headers)

AngularJS���@���q�{���Y�T��,�o���Y�T���N�|��Ҧ����o�e�ШD�ϥ�,���]�t�H�U�T��:
    1.Accept: application/json, text/plain, /
    2.X-Requested-With:XMLHttpRequest

�p�G�A�Q�]�w����S�w���Y�T��,�o�঳��ؤ�k�Ӱ��o��ơG

�Ĥ@�ؤ�k,�p�G�A�۹�Ҧ����o�e�ШD���ϥγo�ǯS�w�Y�T��,���A�ݭn��S�w���T���]�w��Angular�q�{�Y�T�����@����.�i�H�b`$httpProvider.defaults.headers`�t�m�ﹳ�̭��]�w�o��,�o�ӨB�J�q�`�|�b�A��app�]�wconfig�����Ӱ�.�ҥH�p�G�A�Q����"Requested-With"�Y�T���B��Ҧ���GET�ШD�ҥ�"DO NOT TRACK"�]�w,�A�i�H²��a�g�ѥH�U�N�X�Ӱ�:

    angular.module('MyApp',[]).
        config(function($httpProvider) {
            // Remove the default AngularJS X-Request-With header
            delete $httpProvider.default.headers.common['X-Requested-With'];
            // Set DO NOT TRACK for all Get requests
            $httpProvider.default.headers.get['DNT'] = '1';
    });
    
�p�G�A�u�Q��Y�ӯS�w���ШD�]�w�Y�T��,�Ӥ��O�]�w�q�{�Y�T��.����A�i�H�g�ѵ�$http�A�ȶǻ��]�t���w�Y�T����config�ﹳ�Ӱ�.�ۦP���Ȼs���Y�T���i�H�@���ĤG�ӰѼƶǻ���GET�ШD,�Ĥ@�ӰѼƬOURL�r�Ŧ�G
    
    $http.get('api/user', {
    // Set the Authorization header. In an actual app, you would get the auth
    // token from a service
    headers: {'Authorization': 'Basic Qzsda231231'},
    params: {id: 5}
    }).success(function() { // Handle success });
    
�p��b���Τ��B�z�v�������Y�T���������d�ұN�|�b�ĤK����Cheetsheets�d�ҳ������X.

###�֨��^�����

AngularJS��HTTP GET�ШD���ѤF�@�Ӷ}�c�Y�Ϊ�²��֨��t��.�ʬٱ��p�U,����Ҧ����ШD���O�T�Ϊ�,���O�p�G�A�Q��A���ШD�ҥΧ֨��t�ΡA�A�i�H�ϥΥH�U�N�X:

    $http.get('http://server/myapi', {
        cache: true
    }).success(function() { // Handle success });

�o�q�N�X�ҥΤF�֨��t�ΡA�M��AngularJS�N�|�֨��Ӧ�Server���^�����.����ۦP��URL���ШD�ĤG���o�X��,AngularJS�N�|�q�֨��̭����X�e�@�����^����Ƨ@���^����^.�o�ӧ֨��t�Τ]�ܴ���,�Y�ϧA�P�ɹ�ۦPURL�o�X�h�ӽШD,�u���@�ӽШD�|�o�VServer,�o�ӽШD���^����ƱN�|���X���Ҧ�(�P�ɵo�_��)�ШD�C

�M�ӳo�ذ��k�q�i�Ωʪ����׬ݥi��O���ҽĬ�,��@�ӥΤ᭺���ݨ��ª����G,�M��s�����G��M�_�X�ӡA��p�@�ӥΤ�i��Y�N�����@�Ӹ�ƶ�,�ӹ�ڤW�o�Ӹ�ƶ���x�w�g�o�ͤF�ܤ�.

�`�N�Ҧ��^��(�Y�ϬO�q�֨��̨��X��)����W���¬O�D�P�B�^��.���y�ܻ��A����A���Q�Χ֨��^���ɪ��D�P�B�N�X�B�椴�©M�L�V��x���A���o�X�ШD�ɪ��N�X�B�����O�@�˪�.

###��ШD(Request)�M�^��(Response)����ƩҰ����ഫ

AngularJS��Ҧ�`$http`�A�ȵo�_���ШD�M�^�����@�ǰ򥻪��ഫ,���̥]�A:

+ �ШD(Request)�ഫ:
    �p�G�ШD��Cofig�t�m��H��data�ݩʥ]�t�@�ӹ�H�A�N�|��o�ӹ�H�ǦC�Ƭ�JSON�榡.
+ �^��(Response)�ഫ:
    �p�G������@��XSRF�Y,�⥦������.�p�G�^����ƳQ������JSON�榡,��JSON�ѪR���⥦�ϧǦC�Ƭ�JSON�ﹳ.

�p�G�A�ݭn�����t���q�{���Ѫ��ഫ,�Ϊ̷Q�ϥΧA�ۤv���ഫ,�A�i�H��A���ഫ��Ƨ@��Config�t�m��H���@�����ǻ��i�h(�᭱���ӭz).�o���ഫ��Ʊo��HTTP�ШD�MHTTP�^������ƥD��H�Υ��̪��Y�T��.�M���ǦC�ƪ��ק�᪩����^�X��.�bConfig�ﹳ�̭��t�m�o�Ǩ�ƻݭn�ϥΡPtransformRequest�P��M�PtransformResponse�P��,�o�ǳ��i�H�g�Ѩϥ�`$httpProvider�P�A�Ȧb�Ҳժ�config��ƨ����t�m��.

�ڭ̤���ɭԨϥγo�ǭ�?���ڰ��]�ڭ̦��@�Ӧ��A���A����ߺD��jQuery�B�檺�覡.���i��Ʊ�ڭ̪�POST��ƥH`key1=val1&key2=val2`�r�Ŧꪺ�Φ��ǻ��A�Ӥ��O�H`{key1:val1,key2:val2}`�o�˪�JSON�榡.�o�ӮɭԡA�ڭ̥i��۹�C�ӽШD���o�˪��ഫ,�Ϊ̳�Ӧa�W�[transformRequest�ഫ���,���F�F���o�ӽd�ҳo�˪��ؼ�,�ڭ̱N�n�]�w�@�ӳq��transformRequet�ഫ���,�H�K��Ҧ����o�X�ШD,�o�Ө�Ƴ��i�H��JSON�榡�ഫ����ȹ�r�Ŧ�,�U���N�X�t�ܤF�p�󰵳o�Ӥu�@:

    var module = angular.module('myApp');
    module.config(function ($httpProvider) {
        $httpProvider.defaults.transformRequest = function(data) {
            // We are using jQuery�zs param method to convert our
            // JSON data into the string form
            return $.param(data);
       };
    });

##�椸����

�ثe����A�ڭ̤w�g�A�Ѧp��ϥ�`$http`�A�ȥH�Φp��H�i�઺�覡���A�ݭn���t�m.���O�p��g�@�ǳ椸���ըӫO�ҳo�ǰ��u�꦳�Ī��B���?

���p�ڭ̴��g�T�f���������쪺����,AngularJS�@���H���լ�������h�ӳ]�p.�ҥHAngualr���@�Ӽ������A����ݡA�b�椸���դ�,���i�H���A�N�i�H���էA�o�X���ШD�O�_���T,�Ʀܥi�H��T��������^���p��o��B�z,����ɭԱo��B�z.

���ڭ̱����@�U�U���o�˪��椸���ճ���:�@�ӱ���V���A���o�_�ШD,�q���A���o����,�⥦�ᵹ�@�ΰ줺���ҫ�,�M��H���骺�˪O�榡��ܥX��.

�ڭ̪�`NameListCtrl`����O�@�ӫD�`²�檺���.�����s�b�u���@�ӥت��G�X��`names`API���f�A�M���o���Ʀs�x�b�@�ΰ�scope�ҫ���.

    function NamesListCtrl($scope, $http) {
        $http.get('http://server/names', {params: {filter: �ynone�z}}).
            success(function(data) {
                $scope.names = data;
        });
    }

��˹�o�ӱ�����椸���աH�b�ڭ̪��椸���դ�,�ڭ̥����O�ҤU���o�Ǳ���:

+ `NamesListCtrl`������Ҧ����̿ඵ(�åB���T���o��`�J���o�Ǩ̿�)�n
+ ����[���ɺɥi��֦a�ߨ�o���ШD�q���A���o��names���.
+ ���������T�a��^����Ʀs�x��@�ΰ�scope��`names`�ܼ��ݩʤ�.

�b�ڭ̪��椸���դ��c�y�@�ӱ���ɡA�ڭ̵����`�J�@��scope�@�ΰ�M�@�Ӱ��y��HTTP�A��,�b�c�ش��ձ�����覡�M�Ͳ����c�ر�����覡���O�@�˪�.�o�O���ˤ�k�A���ޥ��ݤW�h�W���I�����C���ڬݤ@�U����N�X�G
    
    describe('NamesListCtrl', function(){
        var scope, ctrl, mockBackend;

        // AngularJS is responsible for injecting these in tests
        beforeEach(inject(function(_$httpBackend_, $rootScope, $controller) {
            // This is a fake backend, so that you can control the requests
            // and responses from the server
            mockBackend = _$httpBackend_;

            // We set an expectation before creating our controller,
            // because this call will get triggered when the controller is created
            mockBackend.expectGET('http://server/names?filter=none').
                respond(['Brad', 'Shyam']);
            scope = $rootScope.$new();

            // Create a controller the same way AngularJS would in production
            ctrl = $controller(PhoneListCtrl, {$scope: scope});
        }));

        it('should fetch names from server on load', function() {
            // Initially, the request has not returned a response
            expect(scope.names).toBeUndefined();
            
            // Tell the fake backend to return responses to all current requests
            // that are in flight.
            mockBackend.flush();
            // Now names should be set on the scope
            expect(scope.names).toEqual(['Brad', 'Shyam�z]);
        });
    });

##�ϥ�RESTful�귽

�P$http�P�A�ȴ��Ѥ@�Ӥ�����h����{�����A�o�_XHR�ШD,���O�P�ɤ]�����ѤF�ܱj���i���ʩM�u��.�b�j�h�Ʊ��p�U,�ڭ̳B�z���O�ﹳ���Ϊ̬O�ʸ˦��@�w�ݩʩM��k����H�ҫ�,��p�a���ӤH��ƪ��۵M�H�ﹳ�Ϊ̫H�Υd�ﹳ.

�b�W���o�˪����p�U�A�p�G�ڭ̦ۤv�c�ؤ@��JS�ﹳ�Ӫ�ܳo�ظ������ﹳ�ҫ��A�����k�N���I����nice.�p�G�ڭ̶ȶȷQ�s��Y�ӹ�H���ݩʡB�O�s�Ϊ̧�s�@�ӹ�H�A���ڭ̦p�����o�Ǫ��A�b���A���ݫ��[��.

`$resource`���n���A���ѳo�د�O.AngularJS resources�i�H���U�ڭ̥H�y�z���覡�өw�q�ﹳ�ҫ��A�i�H�w�q�@�U�o�ǯS�x�G

+ resource�����A����URL
+ �o�ؽШD�`�ΰѼƪ�����
+ (�A�i�H�K�O�۰ʱo��get�Bsave�Bquery�Bremove�Mdelete��k),���F���Ǥ�k�A�A�i�H�w�q�䥦����k�A�o�Ǥ�k�ʸˤF��H�ҫ����S�w�\��M�~���޿�(��p�H�Υd�ҫ���charge()�I�O��k)
+ �^������������(�ƲթΪ̤@�ӿW�߹ﹳ)
+ �Y�T��

------------------------------------------------------
����ɭԧA�i�H��Angular Resources�ե�H

�u���A�����A���ݳ]�I�O�HRESTful�覡���ѪA�Ȫ��ɭԡA�A�~���ӥ�Angular resources�ե�.��p�H�Υd���Ӯר�,�ڭ̱N�Υ��@�������o�@�������Ҥl�A�L�N�]�A�H�U���e:

1. ���a�}`/user/123/card`�o�e�@��GET�ШD�A�N�|�o��Τ�123���H�Υd�C��.
2. ���a�}`/user/123/card/15`�o�e�@��GET�ШD,�N�|�o��Τ�123���H��ID��15���H�Υd�T��
3. ���a�}`/user/123/card`�o�e�@�ӦbPOST�ШD��Ƴ����]�t�H�Υd�T����POST�ШD,�N�|���Τ�123�s�إߤ@�ӫH�Υd
4. ���a�}`/user/123/card/15`�o�e�@�ӦbPOST�ШD��Ƴ����]�t�H�Υd�T����POST�ШD,�N�|��s�Τ�123��ID��5���H�Υd���T��.
5. ���a�}`/user/123/card/15`�@�Ӥ�k��DELETE�������ШD,�N�|�R�����Τ�123��ID��5���H�Υd�����.

-------------------------------------------------------

���F���ӧA���n�D���A���Ѥ@�Ӭd�ߦ��A���ݰT������H,`$resource`�٥i�H���A�ϥΪ�^����ƹ�H�N���L�̬O���[�Ƹ�Ƽҫ��@�ˡA�i�H�ק�L�̡A�٥i�H��A���ק���[�Ʀs�x�U��.

`ngResource`�O�@�ӳ�W���B�i�諸�Ҳ�.�n�Q�ϥΥ��A�A�ݻݭn���H�U�Ʊ��G

+ �b�A��HTML���̭��ޥ�angular-resource.js����ڦa�}
+ �b�A���Ҳը̿�̭��n���復���̿�(�Ҧp,angular.module('myModule',['ngResource'])).
+ �b�ݭn���a��A�`�J$resource�o�Ө̿ඵ.

�b�ڭ̬ݫ�˥�ngResource��k�إߤ@��resource�귽���e�A�ڭ̥��ݤ@�U��˥ΰ򥻪�$http�A�Ȱ��������Ʊ�.��p�ڭ̪��H�Υdresource�A�ڭ̷Q���Ū���B�d�ߡB�O�s�H�Υd�T���A�t�~�٭n�ର�H�Υd�ٴ�.

�o��O�W�z�ݨD�@�ӥi�઺��{�G

    myAppModule.factory('CreditCard', ['$http', function($http) {
        var baseUrl = '/user/123/card';
        return {
            get: function(cardId) {
                return $http.get(baseUrl + '/' + cardId);
            },
            save: function(card) {
                var url = card.id ? baseUrl + '/' + card.id : baseUrl;
                return $http.post(url, card);
            },
            query: function() {
                return $http.get(baseUrl);
            },
            charge: function(card) {
                return $http.post(baseUrl + '/' + card.id, card, {params: {charge: true}});
            }
        };
    }]);

���N�H�W�覡�A�A�]�i�H���P�إߤ@�Ӧb�A�����Τ��l�צp�@��Angular�귽�A�ȡA�N���U���N�X�o�ˡG
    
    myAppModule.factory('CreditCard', ['$resource', function($resource) {
        return $resource('/user/:userId/card/:cardId',
            {userId: 123, cardId: '@id'},
            {charge: {method:'POST', params:{charge:true}, isArray:false});
    }]);

����{�b�A�A�N�i�H����ɭԱqAngular�`�J���̭��ШD�@��CreditCard�̿�A�A�N�|�o��@��Angular�귽,�q�{���p�U�A�o�Ӹ귽�|���Ѥ@�Ǫ�l���i�Τ�k.���5-1�C�X�F�o�Ǫ�l��k�H�ΥL�̪��B��欰�A�o�˧A�N�i�H���D�b���A����˰t�m�Ӱt�X�o�Ǥ�k�F.

���5-1 �@�ӫH�Υdreource
<table>
<thead>
 <tr>
   <th>Resource Function</th>
   <th>Method</th>
   <th>URL</th>
   <th>Expected Return</th>
 </tr>
</thead>
<tbody>
  <tr>
    <td>CreditCard.get({id: 11})</td>
    <td>GET</td>
    <td>/user/123/card/11</td>
    <td>Single JSON</td>
  </tr>
  <tr>
    <td>CreditCard.save({}, ccard)</td>
    <td>POST</td>
    <td>/user/123/card with post data �uccard�v</td>
    <td>Single JSON</td>
  </tr>
  <tr>
    <td>CreditCard.save({id: 11}, ccard)</td>
    <td>POST</td>
    <td>/user/123/card/11 with post data �uccard�v</td>
    <td>Single JSON</td>
  </tr>
  <tr>
    <td>CreditCard.query()</td>
    <td>GET</td>
    <td>/user/123/card</td>
    <td>JSON Array</td>
  </tr>
  <tr>
    <td>CreditCard.remove({id: 11})</td>
    <td>DELETE</td>
    <td>/user/123/card/11</td>
    <td>Single JSON</td>
  </tr>
  <tr>
    <td>CreditCard.delete({id: 11})</td>
    <td>DELETE</td>
    <td>/user/123/card/11</td>
    <td>Single JSON</td>
  </tr>
</tbody>
</table>

���ڭ̬ݤ@�ӫH�Υdresource�ϥΪ��N�X�˨ҡA�o�˥i�H���A�z�Ѱ_��ı�o��L�����.

    // Let us assume that the CreditCard service is injected here
    // We can retrieve a collection from the server which makes the request
    // GET: /user/123/card
    var cards = CreditCard.query();
    // We can get a single card, and work with it from the callback as well
    CreditCard.get({cardId: 456}, function(card) {
        // each item is an instance of CreditCard
        expect(card instanceof CreditCard).toEqual(true);
        card.name = "J. Smith";
        // non-GET methods are mapped onto the instances
        card.$save();
        // our custom method is mapped as well.
        card.$charge({amount:9.99});
        // Makes a POST: /user/123/card/456?amount=9.99&charge=true
        // with data {id:456, number:'1234', name:'J. Smith'}
    });

�e���o�Ӽ˨ҥN�X�̭��o�ͤF�ܦh�Ʊ��A�ҥH�ڭ̱N�|�@�Ӥ@�Ӧa�{�u���Ѩ䤤�����n����:

###resource�귽���n��

�n���A�ۤv��`$resource`�D�`²��A�u�n�I�s�`�J��$resource���,�õ��L�ǤJ���T���ѼƧY�i�C(�A�{�b���Ӥw�g���D�p��`�J�̿�,��a?)

$resource��ƥu���@�ӥ����Ѽ�,�N�O���ѫ�x�귽��ƪ�URL�a�},�t�~�٦���ӥi��Ѽ�:�q�{request�ѼưT���M�䥦���Q�b�귽�W�n�t�m���ʧ@.

�Ъ`�N�G�Ĥ@��URL�a�}�ѼƤ������ܼƸ�ƬO�ѼƤƥi�t�m��(:�_���O�Ѽ��ܼƪ��y�k�Ÿ�,��p`:userId`�H���o�ӰѼƱN�|�Q��ڪ�userId�Ѽ��ܼƨ��N(Ķ�̪`:�g�L�ѼƤ�SQL�y�y���H���ӫܼ��x),��`:cardId`�N�|�QcardId�Ѽ��ܼƪ��ȩҨ��N),�p�G�S������ƶǻ��o�ǰѼ��ܼ�,�����Ӧ�m�N�|�Q�Ŧr�Ũ��N.

��ƪ��ĤG�ӰѼƫh�t�d���ѩҦ��ШD���q�{�Ѽ��ܼưT��.�b�o�ӮרҤ��A�ڭ̵�userId�Ѽƶǻ��@�ӱ`�q:123,cardId�Ѽƫh�󦳷N��,�ڭ̵�cardId�Ѽƶǻ��F�@��"@id"�r�Ŧ�.�o�N���ۦp�G�ڭ̨ϥΤ@�ӱq���A����^����H�ӥB�ڭ̥i�H�I�s�o�ӹ�H�������k(��p$save),����o�ӹ�H��id�ݩʱN�|�Q���X�ӽᵹcardId�r�q.

��ƪ��ĤT�ӰѼƬO�@�ǧڭ̷Q�n���S���䥦��k�A�o�Ǥ�k�O��Ȼs�Ƹ귽���ާ@����k.�b�U�������`�A�ڭ̱N�|�`�װQ�׳o�Ӹ��D

###�Ȼs�Ƥ�k

$resource��ƪ��ĤT�ӰѼƬO�i�諸�A�D�n�ΨӶǻ��n�bresource�귽�W���S���䥦�۩w�q��k�C

�b�o�ӮרҤ��A�ڭ̦۩w�q�F�@�Ӥ�kcharge.�o�Ӧ۩w�q��k�i�H�g�Ѷǻ��@�ӹﹳ�ӳQ�t�m�W.�o�ӹ�H�̦�����ȡA����F����k�����S�W��.�o�Ӱt�m�ݭn���@��request�ШD����k����(GET,POST����)�A�H�θӽШD���ݭn���ѼƤ]�n�Q�ǻ�(��pcharge=true),�åB�n����^��H�O�Ʋ��٬O��Ӵ��q��H�C�o�@����d�w����A�A�N�i�H�b���o�ӷ~�ȹ�ڻݭn�D���ɭԡA�ۥѦa�I�s`CreditCard.charge()`��k.

###���n�ϥΦ^�I��ƾ���!(���D�A�u���ݭn����)

�ĤT�ӻݭn�`�N���Ʊ��O�귽�I�s����^����.���ڭ̦A�����`�@�U`CreditCard.query()`�o�Ө��.�A�N�|�ݨ줣�O�b�^�I��Ƥ���cards���,�ӬO�����⥦�ᵹcard�ܼ�.�b�D�P�B���A���ШD�����p�U���A�o�˪��N�X�O�p��B�@����?

�A��ߥN�X�O�_���`�u�@�O�諸�A���O�N�X��ڤW�O�i�H���`�u�@��.�o�̹�ڵo�ͪ��OAngularJS��ȤF�@�Ӥޥ�(�O���q��H���٬O�Ʋժ����M��A���檺��^����)�A�o�ӤޥαN�|�b���Ӧ��A���ШD�^����^�ɳQ��R.�b�o�����A�o�ӤޥάO�Ӫ�����.

�]���bAngularJS���Τ����j�h�Ƴq�ιL�{���O�q���A���ݨ���ơA�⥦�ᵹ�@���ܼơA�M��b�Ҫ��W��ܥ�,�ӤW���o�˪�²�ƾ���D�`�u��.�b�A������N�X��,�A�Ҧ��ݭn�h�����N�O�o�X���A���ݽШD,���^�Ƚᵹ���T���@�ΰ�(scope)�ܼ�.�M��ѤU���X�A��V�o�Ǹ�ƴN�Ѽ˪O�t�Υh�ޤߤF.

�p�G�A�Q���^�Ȱ��@�Ƿ~���޿�B�z�A���۶��`��k�N���૵�ĤF.�b�o�ر��p�U�A�A�N�o�̿�^�I��ƾ���F�A��p�bCredit.get()�I�s���ϥΪ����ؾ���.

###²�ƪ����A���ݾާ@
















