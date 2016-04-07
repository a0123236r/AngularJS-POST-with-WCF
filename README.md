# AngularJS-POST-with-WCF
client side use angularJS to use $http.post method, server side use WCF POST method


STEP : 1
    Write server side WCF code, detail in WCF file
    
STEP : 2
    Write client side AngularJS code, detail in controller 

STEP : 3
    Test function and REST webservice
    

Remark:
        + if WCF IService BodyStyle = WebMessageBodyStyle.Bare. So JSON date should like this
           [{"Name":"jack", "Value": "22"}, {"Name": "lily", "Value": "25"}]
           
        + if WCF IService BodyStyle = WebMessageBodyStyle.Wrapped. So JSON date should like this
          {"lcc" : [{"Name":"jack", "Value": "22"}, {"Name": "lily", "Value": "25"}]}
          
        + AngularJS controller headers Content-Type should be application/json. Do NOT application/JSON
