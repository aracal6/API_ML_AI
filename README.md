|   发布名称  |  发布时间   |   发布人  |
| --- | --- | --- |
|   安全社区app  |  2019.12.8   |   戴嘉俊  |


## 价值主张设计

#### 加值宣言
- 随着社会发展，房地产的兴起，必定使得出现老社区缺少管理，无规划的问题。针对这一现象，市面上开始出现智能社区app，帮助老城区规划管理，以最低的成本来改善社区居民的安全出行。针对老社区的停车杂乱无章，人员乱入，治安管理成本高的问题，这类app有人脸识别门禁功能，车牌检测功能。但针对到居民个人的功能确没有。所有基于现状，该app将采用基本的人脸识别门禁功能、车牌检测功能保障基本社区安全出行功能之外，还将采用语音合成功能、危险行为识别功能，图像识别功能来为居民的安全出行提供新功能及保障。

- 通过人脸识别功能识别&图像识别功能，方便居民刷脸/身份证出入社区，管理陌生人群进入，达成刷卡管理监控的功能。还能识别陌生人群，危险人群进行预防警报。
- 车牌识别功能对出入车辆进行管理，对不属于本小区的车辆进行禁入管理。
- 语音合成功能针对居民个人用户，在家遇到陌生人/危险人物敲门，女性用户可转换男声播放回应，多人谈话声回应。

|   优先级  |  次优先级 |
| --- | --- |
|   1.基于百度api人脸识别&图像识别功能，通过人脸识别与身份证证件等对社区出入人员进行监控与管理、实现出入自动化。2.基于百度api车牌识别功能，实现对车辆信息的自动识别，可实现无卡、无人的进出场自动化、规范化管理，有效降低人力成本和通行卡证制作成本，提升管理效率  | 3.基于百度api的语音合成功能，将用户的声音或文案转换成男声播放。4.基于危险行为识别，针对监控视频片段，识别其是否有危险行为，进行监控与报警  | 

#### 核心价值
- 本产品着眼于用户的安全居住出行需求，解决老社区停车杂乱无章，人员乱入缺少管制，居住具有安全风险的问题。

#### 核心价值与用户痛点
|   核心价值  |  用户痛点 |
| --- | --- |
|  便捷性 |过去用户出入社区门禁需要携带门禁ic卡，会出现忘带、丢失等情况，造成出行不便。过去车辆的出入需要与保安交涉，证明自己的身份才可进入。现在实现自动化车牌检测出入，减少了出入时间上的浪费。 | 
|  安全性 | 丢失的门禁ic卡。可能会被不法分子拿来谋不法之事。现在实现出入人员的身份验证管理，大大降低了安全隐患。危险行为的的检测监控视频片段，识别危险行为与人群，标记与警监控警惕。语音合成可以在一定程度上保证女性单独居住时的安全。| 

#### 人工智能概率性与用户痛点

#### 需求列表与人工智能API加值
|  用户需求   |   重要性  |    api技术接口 |
| --- | --- | --- |
|  用户通过小区门禁进去小区   |   重要  |   人脸识别&图像识别  |
|  用户驾驶车辆进入小区  |  重要   | 车牌识别    |
|  女性用户语音合成转化播放警告陌生人  |  次重要   | 语音合成    |
|  针对监控视频识别危险行为  |  次重要   | 危险行为检测    |

具体使用场景：
1.小明下班回家，想通过门禁进入小区，但是忘带了门禁卡，这时注意到小区门口新安装的门禁系统，记起早前小区录入了居民人脸信息，走上前刷脸进入。

2.小明出门远行，今天开车回家，来到小区门口，正当想和熟悉的保安叔叔打招呼开栏杆进入小区时，车窗还没摇下，栏杆就自动上升允许通过了。开过保安亭时，发现保安叔叔不在，他产生了疑惑。这时他注意到了车栏杆旁的摄像头，意识到早前小区录入了居民车牌，原来是新装的车牌检测系统自动化检测车辆出入。不禁感叹科技的方便。

3.小红是一位单身的职场女性，今天她像平时一样一个人下班回家。深夜的时候，门口突然想起一阵急促的敲门声，门外一个陌生的声音喊道半夜查水表。这时小红打开手机app，使用语音合成功能，将文案输出，调整语速、性别播放回应门外的陌生人。陌生人听到是男性声音后，找借口离去。

4.


## 三、API 产品使用及输出展示

#### 1、API展示说明及输出
（1）人脸识别--人脸搜索api
- 接口描述：面对镜头，对比人脸库中N张人脸，进行1：N检索，找出最相似的一张或多张人脸，并返回相似度分数。支持百万级人脸库管理，毫秒级识别响应，可满足身份核验、刷脸通行等应用场景
- 接口地址：[百度ai人脸搜索api文档](https://ai.baidu.com/ai-doc/FACE/Gk37c1uzc)
- 请求URL数据格式：向API服务地址使用POST发送请求
- 请求url：https://aip.baidubce.com/rest/2.0/face/v3/search
- 输入代码
```
# encoding:utf-8

import requests

'''
人脸搜索
'''

request_url = "https://aip.baidubce.com/rest/2.0/face/v3/search"

params = "{\"image\":\"027d8308a2ec665acb1bdf63e513bcb9\",\"image_type\":\"FACE_TOKEN\",\"group_id_list\":\"group_repeat,group_233\",\"quality_control\":\"LOW\",\"liveness_control\":\"NORMAL\"}"
access_token = '24.c2c1012eb8ae7a9379a84df7b6e11c4f.2592000.1579705577.282335-17258797'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/json'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```

- 输出代码
```
  { "face_token": "fid", "user_list": [{"group_id" : "test1","user_id": "u333333","user_info": "Test User","score": 99.3 }]}
  #输出的结果数值
  
```

  - score的值表示用户的匹配得分，数值越高证明匹配成功推荐的阈值是80，用户score输出值达80以上即可通过
  
  
  （2）百度api车牌识别
  - 文字识别--车牌识别技术
  - 接口描述：对机动车蓝牌、绿牌、单/双行黄牌的地域编号和车牌号进行识别，并能同时识别图像中的多张车牌。
  - 接口地址：[百度ai车牌识别api文档](https://ai.baidu.com/ai-doc/OCR/ck3h7y191)
  - 请求方式：请求URL数据格式：向API服务地址使用POST发送请求
  - 请求url：https://aip.baidubce.com/rest/2.0/ocr/v1/license_plate
  - 输入代码
```
def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()


#获取车牌号信息
def get_license_plate(path):

    request_url = "https://aip.baidubce.com/rest/2.0/ocr/v1/license_plate"
    
    f = get_file_content(path)
    access_token=('24.c2c1012eb8ae7a9379a84df7b6e11c4f.2592000.1579705577.282335-17258797')
    img = base64.b64encode(f)
    params = {"custom_lib": False, "image": img}
    params = urllib.parse.urlencode(params).encode('utf-8')
    request_url = request_url + "?access_token=" + access_token
    request = urllib.request.Request(url=request_url, data=params)
    request.add_header('Content-Type', 'application/x-www-form-urlencoded')
    response = urllib.request.urlopen(request)
    content = response.read()
    if content:
        license_plates = json.loads(content.decode("utf-8"))
        strover = '识别结果：'
        words_result = license_plates['words_result']
        number = words_result['number']
        strover += '  车牌号：{} \n '.format(number)
#        print (content)
        print (strover)
        return content
    else:
        return ''

image_path='C:\Users\dai\Desktop\车牌.png'
get_license_plate(image_path)
```

- 输出代码
```
{"errno": 0,"msg": "success","data": {"log_id": "5327722537189137631","words_result": {"color": "green","number": "京KBT355","probability": [1,0.9999977350235,0.99999630451202,0.99999868869781,0.99998331069946,0.99999988079071,0.9531751871109,0.99922955036163],"vertexes_location": [{"y": 223,"x": 170},{y": 223,"x": 282},{"y": 256,"x": 282},{"y": 256,"x": 170}]}}}
```
  

  
  
  
  
  
