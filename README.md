|   发布名称  |  发布时间   |   发布人  |
| --- | --- | --- |
|   易出行（安全社区app）  |  2019.12.8   |   戴嘉俊  |

### 20x20 ppt https://github.com/aracal6/API_ML_AI/blob/master/20x20(1)(1).pptx
## 价值主张设计  

#### 加值宣言
- 随着社会发展，房地产的兴起，新小区的日益增多，老社区渐渐地埋没在人们的视线中，随着社区的设备老化，管理者的投资减少，老社区出现了缺少管理，无规划的问题。针对这一现象，市面上开始出现智能社区app，帮助老城区规划管理，以最低的成本来改善社区居民的安全出行。针对老社区的停车杂乱无章，人员乱入，治安管理成本高的问题，这类app有人脸识别&身份证识别功能。但针对到居民个人的功能确没有。所以基于现状，该app将采用基本的人脸识别&图像识别门禁功能、车牌检测功能保障基本社区安全出行。

- 通过人脸识别功能识别&图像识别功能，方便居民刷脸/身份证出入社区，管理陌生人群进入，达成刷卡管理监控的功能。还能识别陌生人群，危险人群进行预防警报。
- 车牌识别功能对出入车辆进行管理，车辆进出系统录入上传登记，车位实时显示。


|   优先级  |  次优先级 |
| --- | --- |
|   1.基于百度api人脸识别&图像识别功能，通过人脸识别与身份证证件等对社区出入人员进行监控与管理、实现出入自动化。2.基于百度api车牌识别功能，实现对车辆信息的自动识别，可实现无卡、无人的进出场自动化、规范化管理，有效降低人力成本和通行卡证制作成本，提升管理效率  | 3.车牌识别功能，登记进出车辆，实时显示剩余车位  | 

#### 核心价值
- 本产品着眼于用户的安全居住出行需求，解决老社区停车杂乱无章，人员乱入缺少管制，居住具有安全风险的问题。

#### 核心价值与用户痛点
|   核心价值  |  用户痛点 |
| --- | --- |
|  便捷性 |过去用户出入社区门禁需要携带门禁ic卡，会出现忘带、丢失等情况，造成出行不便。过去车辆的出入需要与保安交涉，证明自己的身份才可进入。现在实现自动化车牌检测出入，减少了出入时间上的浪费。 | 
|  安全性 | 丢失的门禁ic卡。可能会被不法分子拿来谋不法之事。现在实现出入人员的身份验证管理，大大降低了安全隐患。| 

#### 人工智能概率性与用户痛点
- 人脸库管理
提供可视化人脸库管理功能，支持人脸组、用户、人脸维度的增、删、改、查操作 

- 身份证识别
提供移动端SDK，使用时能实时检测取景框中是否包含身份证，是否存在模糊、欠/过曝等情况，并提示用户矫正，提高采集质量，提升准确率 
- 车牌识别
依托百度优秀的图像处理技术和海量优质数据，支持识别多种常见类型车牌信息，对蓝牌、绿牌、单/双行黄牌识别准确率可达95%以上 

- 人脸识别--人脸搜索
人脸的姿态角度、遮挡度、清晰度、光照条件，确保输入的图片符合质量标准即可保证高准确度的判断
万级别人脸库首选识别率高达99%以上，索速度业内领先

###### 但人工智能再出色也会存在偏差情况

![人脸搜索.png](https://upload-images.jianshu.io/upload_images/9643258-9b208f860f4fe4ef.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 多人同时检测会下降识别准确度，并无法判断单一主体

![多人识别.png](https://upload-images.jianshu.io/upload_images/9643258-3446623f0725cfb0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


###### 为了更好地、更精确地解决用户痛点。针对人工智能概率性，app增加提醒功能，提醒用户使用人脸/身份证/车牌识别功能时，弹窗提示当前环境过于光亮/昏暗/不清晰等影响准确率的条件，提高api识别准确率。



#### 需求列表与人工智能API加值
|  用户需求   |   重要性  |    api技术接口 |
| --- | --- | --- |
|  用户通过小区门禁进去小区   |   重要  |   人脸识别&图像识别  |
|  用户驾驶车辆进入小区  |  重要   | 车牌识别    |
|  外来人员进入小区  |  重要   | 人脸识别&图像识别    |

具体使用场景：
1.小明下班回家，想通过门禁进入小区，但是忘带了门禁卡，这时注意到小区门口新安装的门禁系统，记起早前在易出行app上录入了自己的人脸信息，打开app一键开门。

2.小明出门远行，今天开车回家，来到小区门口，正当想和熟悉的保安叔叔打招呼开栏杆进入小区时，车窗还没摇下，栏杆就自动上升允许通过了。开过保安亭时，发现保安叔叔不在，他产生了疑惑。这时他注意到了车栏杆旁的摄像头，意识到早前在易出行app里录入了自己的车牌号码，原来是新装的车牌检测系统自动化检测车辆出入。不禁感叹科技的方便。

3.新来的外卖小哥小王接到外卖单送往光明小区，因没有送过该小区，担心小区保安询问导致配送超时，这是他注意到小区门口的门禁系统，拿出身份证直接刷卡通过，减去了与保安叔叔交涉的时间，配送顺利到达。




## 二、产品设计原型

#### 产品架构图
![aa957429e9e6c1b4b2fb6c832d1341d.png](https://upload-images.jianshu.io/upload_images/9643258-64be60090bcf8922.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 1、交互及界面设计
##### 手机端
- 注册登录

![30ae961e69bc0b84487b6dcb3b2c09d.png](https://upload-images.jianshu.io/upload_images/9643258-7749a8872bef7ce9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 个人中心

![35e8060b086d538870304686890777c.png](https://upload-images.jianshu.io/upload_images/9643258-953267449af25100.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


- 功能区

![84b81a482f9e97b93d09dda2b4f9e80.png](https://upload-images.jianshu.io/upload_images/9643258-f89e9ed5f32328e7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


- 社区管理中心

![ce29a8ea538a27c67cd34b6f4413c6a.png](https://upload-images.jianshu.io/upload_images/9643258-f4d64617810f9744.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



##### 终端

![b987946b6d7851330911d6b8c071d59.png](https://upload-images.jianshu.io/upload_images/9643258-3421c4709b4a7f1b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


#### 2.信息设计
- 终端信息返回

![57a3a5c170c8b9cdcdb1c7bf4a03f96.png](https://upload-images.jianshu.io/upload_images/9643258-4cf8af5ebe546011.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- app端信息返回

![35e8060b086d538870304686890777c.png](https://upload-images.jianshu.io/upload_images/9643258-12aa76084a3ea995.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


#### 3.原型文档
- 1.原型html链接：http://aracal6.gitee.io/easy-to-travel
- 2.原型文件下载：https://gitee.com/aracal6/Easy-to-travel

#### 4.口头操作说明
易出行是一款方便居民出入小区，改善社区安全保障问题及提升居民居住安全感的app。
针对用户只要在app上绑定自己的小区，上传自己的人脸信息、身份证和车牌号码即可日后一键开小区门禁锁，车辆出入自动识别。最大程度的便捷你的生活。
针对社区管理，社区管理者可以在app上修改车辆、居民信息。保障信息的录入，可以通过扫描和云数据录入，操作简单便捷。






## 三、API 产品使用及输出展示

#### 1、API展示说明及输出
（1）人脸库管理
- 接口描述：人脸库管理相关接口，要完成1：N或者M：N识别，首先需要构建一个人脸库，用于存放所有人脸特征。
- 图片格式：现支持PNG、JPG、JPEG、BMP，不支持GIF图片
- 请求URL数据格式：向API服务地址使用POST发送请求
- 请求url：https://aip.baidubce.com/rest/2.0/face/v3/faceset/user/add
- 输入代码
```
# encoding:utf-8

import requests

'''
人脸注册
'''

request_url = "https://aip.baidubce.com/rest/2.0/face/v3/faceset/user/add"

params = "{\"image\":\"027d8308a2ec665acb1bdf63e513bcb9\",\"image_type\":\"FACE_TOKEN\",\"group_id\":\"group_repeat\",\"user_id\":\"user1\",\"user_info\":\"abc\",\"quality_control\":\"LOW\",\"liveness_control\":\"NORMAL\"}"
access_token = '24.c2c1012eb8ae7a9379a84df7b6e11c4f.2592000.1579705577.282335-17258797'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/json'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())

```

- 输出代码：
```
{
  "face_token": "2fa64a88a9d5118916f9a303782a97d3",
  "location": {
      "left": 117,
      "top": 131,
      "width": 172,
      "height": 170,
      "rotation": 4
  }
}
```


（2）人脸识别--人脸搜索api
- 接口描述：面对镜头，对比人脸库中N张人脸，进行1：N检索，找出最相似的一张或多张人脸，并返回相似度分数。支持百万级人脸库管理，毫秒级识别响应，可满足身份核验、刷脸通行等应用场景
- 接口地址：[百度ai人脸搜索api文档](https://aip.baidubce.com/rest/2.0/face/v3/search)
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
  
  （3）百度api身份证识别
  - 文字识别--身份证识别
  - 接口描述：支持对大陆居民二代身份证正反面的所有字段进行结构化识别，包括姓名、性别、民族、出生日期、住址、身份证号、签发机关、有效期限；并支持检测身份证正面的头像信息，并返回其位置及头像切片的 base64 编码。 同时，支持对用户上传的身份证图片进行图像风险和质量检测，可识别图片是否为复印件或临时身份证，是否被翻拍或编辑，是否存在正反颠倒、模糊、欠曝、过曝等质量问题。
  - 接口地址：[百度ai身份证识别api文档](https://ai.baidu.com/ai-doc/OCR/rk3h7xzck)
  - 请求方式：请求URL数据格式：向API服务地址使用POST发送请求
  - 请求url：https://aip.baidubce.com/rest/2.0/ocr/v1/idcard
  - 输入代码
  ```
# encoding:utf-8

import requests
import base64

'''
身份证识别
'''

request_url = "https://aip.baidubce.com/rest/2.0/ocr/v1/idcard"
# 二进制方式打开图片文件
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"id_card_side":"front","image":img}
access_token = '24.c2c1012eb8ae7a9379a84df7b6e11c4f.2592000.1579705577.282335-17258797'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
  ```
  
  - 输出代码
  ```
  {"log_id": 2648325511,"direction": 0,"image_status": "normal","idcard_type": "normal","edit_tool": "Adobe Photoshop CS3 Windows","photo": "/9j/4AAQSkZJRgABA......","photo_location": {"width": 1189,"top": 638,"left": 2248,"height": 1483},"words_result": {"住址": {"location": {"left": 267,"top": 453,"width": 459,"height": 99},"words": "南京市江宁区弘景大道3889号"},"公民身份号码": {"location": {"left": 443,"top": 681,"width": 589,"height": 45},"words": "330881199904173914"},"出生": {"location": {"left": 270,"top": 355,"width": 357,"height": 45},"words": "19990417"},"姓名": {"location": {"left": 267,"top": 176,"width": 152,"height": 50},"words": "伍云龙"},"性别": {"location": {"left": 269,"top": 262,"width": 33,"height": 52},"words": "男"}"民族": {"location": {"left": 492"top": 279,"width": 30,"height": 37},"words": "汉"}},"words_result_num": 6}
  ```
  
  
  
  
  （4）百度api车牌识别
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

- 输入代码
```
{"errno": 0,"msg": "success","data": {"log_id": "5327722537189137631","words_result": {"color": "green","number": "京KBT355","probability": [1,0.9999977350235,0.99999630451202,0.99999868869781,0.99998331069946,0.99999988079071,0.9531751871109,0.99922955036163],"vertexes_location": [{"y": 223,"x": 170},{y": 223,"x": 282},{"y": 256,"x": 282},{"y": 256,"x": 170}]}}}
```
  


#### 2.使用比较分析
|     |   百度AI人脸库管理|  腾讯云人脸库管理 |
| --- | --- | --- |
|   链接  |   [百度AI人脸库管理](https://ai.baidu.com/ai-doc/FACE/7k37c1twu)  |  [腾讯云人脸库管理](https://cloud.tencent.com/document/product/867/32780) |
|   价格  | 300元/月/QPS、30元/天/QPS | 3100元/100万次 | 
|   特点  |   添加人脸无上限  | 最多包含1000万张人脸   |




|     |   百度AI人脸识别-搜索API  |  腾讯云ai人脸识别-搜索   | Face++人脸搜索   |
| --- | --- | --- |--- |
|   链接  |   [百度AI人脸识别-搜索API](https://ai.baidu.com/tech/face/search)  |  [腾讯云ai人脸识别-搜索](https://ai.qq.com/product/face.shtml#search)   | Face++人脸搜索](https://www.faceplusplus.com.cn/)   |
|   价格  | 300元/月、30元/天  |  0.0032元/次、3100元/100万次 | 0.01/次、100元/天、1000元/月 |
|   准确率  |   90%以上  |  80%以上   |  90%以上  |
|   优点  |   提供可视化人脸库管理功能，支持人脸组、用户、人脸维度的增、删、改、查操作 | 支持大角度侧脸、快速移动人脸   |  数值返回多样化属性分析、还包括皮肤状态  |
|   缺点  |   多个人脸检索识别率会下降 |  搜索对比识别率较低   |  搜索对比识别率较低   |






|     |   百度AI文字识别-身份证识别 |  腾讯云身份证ocr   |  Face++身份证识别 |
| --- | --- | --- |--- |
|   链接  |   [百度AI文字识别-身份证识别](https://ai.baidu.com/tech/ocr_cards/idcard)  |  [腾讯云身份证ocr](https://ai.qq.com/product/ocr.shtml#identify)   | [Face++身份证识别](https://www.faceplusplus.com.cn/idcard-recognition/) |
|   价格  | 每日500免费调用、200元/一万次、0.02元/次 | 120元/1000次 |  0.01元/次、1000元/每月（1QPS）|
|   准确率  |  超过99%   | 中文98%以上，数字99%以上   |  99%以上  |
|   优点  |   高识别率，支持识别各角度身份证照片，对少数民族身份证进行专项优化 | 适应各种实际应用中的异常情况，如光照不均、倾斜、模糊等，具备非常高的复杂环境可用性   |           |  翻拍、PS等真实性识别 |
|   缺点  |   在复杂的使用环境下识别率下降 | 在复杂的使用环境下识别率下降  | 翻拍、PS等真实性识别 |





|     |   百度AI车牌识别 |   Face++车牌识别 |
| --- | --- | --- |
|   链接  |   [百度AI车牌识别](https://ai.baidu.com/tech/ocr_cars/plate)  |  [Face++车牌识别](https://www.faceplusplus.com.cn/license-plate-recognition/) |
|   价格  | 每日200次免费调用、0.009元/次起步 | 0.01元/次、100元/天、1000元/月 | 
|   准确率  |  95%   | 95%   | 
|   优点  |   准确率高，适应不同场景  | 精准识别，适应不同光照场景，适应倾斜/模糊等场景   |
|   缺点  |  无  |  无 | 







#### 3.使用后风险报告
（1）人脸库管理
- 价格：百度<腾讯
- 优点比较：百度的人脸库人脸添加是没有上限，腾讯的人脸库添加上限1000万，但对于小区来说，1000万以下的数量绰绰有余。两家的人脸库增删改查功能都齐全，差异不大，所以使用哪家的人脸库api取决于人脸搜索api功能更加强大。（因选择了百度人脸搜索api，所以使用百度人脸库管理，原因如下）


（2）人脸识别-搜索api
- 价格：百度<face++<腾讯
- 准确率：根据三家的api使用情况准确率情况，百度与face++的准确率较高，基本能够识别出不同表情下的人脸，但是根据实际使用情况，模糊了照片和光线等，则会出现不同程度的识别错误。
- 根据实际场景使用的准确度比较，三家的差别并没有特别大，综合价格、准确度决定产品人脸搜索功能使用百度api。

（3）身份证识别
- 价格：百度<face++<腾讯
- 准确率：根据三家的使用情况比较，准确率差别不大，都有95%以上的识别率保障。
- 根据两个条件的综合对比，百度身份证识别价格取胜，每日500次的免费调用，单次0.02元的低价，降低了使用成本。


（4）车牌识别
- 价格：百度<face++
- 准确度：两家准确率无差异，均能满足日常使用。
- 根据性价比，百度占明显优势，决定使用百度车牌识别api


##### 选择的api在产品中的可行性与未来发展性
- 百度api的服务平台稳定，使用一体化的人脸管理与搜索，有利于后台数据的优化及提高响应速度。
- 4款api技术性不高，能够精准解决社区面临的安全问题，以最低成本、最快捷的方式精确地解决了用户痛点。
- 根据市场可行性，市面上已经出现了类似的app，在小区中还没有大量投入使用，该产品还附带一键开门功能与车辆管理功能，是当前市面上产品的缺少的优势。

#### 4.加分项
- 该产品使用了两种以上api
- [百度AI人脸库管理](https://ai.baidu.com/ai-doc/FACE/7k37c1twu)
- [百度AI人脸识别-搜索API](https://ai.baidu.com/tech/face/search)
- [百度AI文字识别-身份证识别](https://ai.baidu.com/tech/ocr_cards/idcard) 
- [百度AI车牌识别](https://ai.baidu.com/tech/ocr_cars/plate)
