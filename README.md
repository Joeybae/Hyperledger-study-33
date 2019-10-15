# Hyperledger-study-33

하이퍼레져 앱 만들기 실습 33일차 - object 형식, object 반복문, object 값으로서 함수

출처 : https://opentutorials.org/course/3332/21145

1. object 형식 - syntax/object.js

        var members = ['egoing', 'k8805', 'hoya'];
        console.log(members[1]); // k8805

        var roles = {
          'programmer':'egoing',
          'designer' : 'k8805',
          'manager' : 'hoya'
        }
        console.log(roles.designer); //k8805

2. object 반복문 - syntax/object.js

        var members = ['egoing', 'k8805', 'hoya'];
        console.log(members[1]); // k8805
        var i = 0;
        while(i < members.length){
          console.log('array loop', members[i]);
          i = i + 1;
        }

        var roles = {
          'programmer':'egoing',
          'designer' : 'k8805',
          'manager' : 'hoya'
        }
        console.log(roles.designer); //k8805
        console.log(roles['designer']); //k8805

        for(var n in roles){
          console.log('object => ', n, 'value => ', roles[n]);
        }

3. object 값으로서 함수 - syntax/object2.js

        var f = function(){
          console.log(1+1);
          console.log(1+2);
        }
        var a = [f];
        a[0]();

        var o = {
          func:f
        }
        o.func();
