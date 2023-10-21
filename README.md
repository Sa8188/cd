var data =a.getQuestion(1);
function call(){
    var len = data.length;
    for(var i = 0 ;i<len;i++){
        var id = data[i][3] ;
        var flag= 0 ;
        for(var j =10;j<14;j++){
            if(id == data[i][j][0]){
                console.log(i+1,data[i][j][1]);
                flag = 1 ;
            }
        }
        if(flag == 0)
            console.log(i+1,'E');
    }
}
call();
