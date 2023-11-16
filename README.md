# FlaskAppCodeDeploy

 flask app을 CodeDeploy를 이용해서 EC2 인스턴스에 배포 실습


1. 플라스크 파이썬 파일 제작

c:\aws> mkdir hello-flask

c:\aws> cd hello-flask

c:\aws\hello-flask> code .

------------------------------

from flask import Flask
app = Flask(__name__)


@app.route('/hello')
def hello():
    return 'hello flask & code deploy'


if __name__ == '__main__':
    app.run()
    
------------------------------

c:\aws\hello-flask> python -m venv venv

c:\aws\hello-flask> .\venv\Scripts\activate

2. 깃허브 레포지터리 생성 후 소스 등록

3. 필요한 yml 파일 등 확인?
