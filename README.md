# lambda
import json

def lambda_handler(event, context):
    # TODO implement
    return {
        'statusCode': 200,
       # 'body': json.dumps('Hello from Hedy!!!')
       "body":event
    }
#Request Body(test)
#{
  #"key1": "value1",
  #"key2": "value2",
  #"key3": "value3"
#}
#lambda function located debug 的動作使用AWS其他服務，核心競爭是無伺服器，無須擔心memory、CPU不夠，也無須擔心硬體設備，讓客戶專心開發程式
#lambda+RDS讓DNS更自動化，例如:員工自動填完jira表單，從lambda function存到RDS，公司再掃描RDS讀取資料、設定DNS即可，增加IT自動化流程
#RDS關聯性資料庫
#顛覆傳統搭建資料庫需考慮實體主體維護硬體設施、資料庫後續管理；快速搭建關聯性資料庫，並且後續維護、自動備份；在流量大時，可把流量擴展，消除當機卡關風險
#API gateaway
#tigger:{"statusCode": 200, "body": "\"Hello from Hedy!!!\""}
#S3
#透過API gateaway建立一格API把使用者上傳圖片需求傳到S3
#S3、gateaway 
#例如:資安，把程序包裝成程式檔，讓員工按程式按鈕，程式會把圖自動上傳到搭建的bucket中
