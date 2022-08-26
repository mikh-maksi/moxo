# moxo

About elements for developing.
## BackEnd. Data Scheme
#### Input of black box  
**/getusers**
[
    {level_num:1,sublevel:1,indexinsub:1,from_test_time_ms:0,to_test_time_ms:4000,stimulus_duration_ms:4000,test_id:1003682,age_group:1,rtime1:0,rtime2:0,a_clicks:1,t_clicks:1,h_clicks:0,i_clicks:0,total_clicks:1,status1:"GP",status2:,id:0,global_time:105384676},
    
    {level_num:1,sublevel:1,indexinsub:1,from_test_time_ms:0,to_test_time_ms:4000,stimulus_duration_ms:4000,test_id:1003682,age_group:1,rtime1:0,rtime2:0,a_clicks:1,t_clicks:1,h_clicks:0,i_clicks:0,total_clicks:1,status1:"GP",status2:,id:0,global_time:105384676}
]

**/getuser**
    {level_num:1,sublevel:1,indexinsub:1,from_test_time_ms:0,to_test_time_ms:4000,stimulus_duration_ms:4000,test_id:1003682,age_group:1,rtime1:0,rtime2:0,a_clicks:1,t_clicks:1,h_clicks:0,i_clicks:0,total_clicks:1,status1:"GP",status2:,id:0,global_time:105384676}


#### Output of BlackBox

{"id":1174,"name":"Hyperactivity","issue_id":400,"age1":10,"age2":11,"gender":M,"avg":13.66,"std":6.81,"indicator_1":1.65,"created":2011-12-25 10:51:49.000,"modified":2011-12-25 10:51:49.000,"norm_key":H,"country_id":999,"l1_avg":2.416666667,"l1_std":2.665922515,"l2_avg":2.694444444,"l2_std":2.713136766,"l3_avg":3.0,"l3_std":2.917924899,"l4_avg":1.888888889,"l4_std":1.894017314,"l5_avg":2.083333333,"l5_std":2.143095225,"l6_avg":2.055555556,"l6_std":2.437146393,"l7_avg":1.805555556,"l7_std":2.412105712,"l8_avg":1.555555556,"l8_std":1.611466846,"severity_1":-1.65,"severity_2":-1.95,"severity_3":-2.25,"severity_4":-2.55
}


#### Needed structure

{id:1784642,subscription_id:1784517,patient_id:1784635,customer_id:1784514,created:23:52.0,modified:44:20.0,metric_a:248,metric_t:153,metric_h:29,metric_i:21,name:Test,medication_id:1327,other_medication:"",dosage:0,severity_a:0,severity_t:1,severity_h:0,severity_i:1,indicator_a:2,indicator_t:3,indicator_h:2,indicator_i:3,status_id:100,focus_table:"[{""BHPTot"":2,""BHPAvr"":""0.519"",""BHVTot"":0,""attenTotWithGVP"":32,""BHVAvr"":0,""GVPTot"":10,""VPTot"":10,
""attenAvrWithGVP"":""0.448"",""VPAvr"":""0.176"",""BAPTot"":1,""impulseAvr"":""0.490"",""BAPAvr"":""0.490"",""BPTot"":1,
""missTot"":1,""BPAvr"":""20.060"",""impulseTot"":1,""attenTot"":22,""attenAvr"":""0.571"",""attenGrade"":56,""impulseGrade"":90,
""lvlDistType"":""Basic1"",""hyperAvr"":""7.033"",""hyperGrade"":70,""hyperTot"":3,""hyperTotWithBHV"":3,""attenGradeWitnGVP"":92,
""hyperAvrWithBHV"":""7.033"",""GPTot"":22,""hyperGradeWithBHV"":70,""GPAvr"":""0.571"",""lvlNum"":1,""GVPAvr"":""0.176""},
{""BHPTot"":0,""BHPAvr"":0,""BHVTot"":1,""attenTotWithGVP"":31,""BHVAvr"":""0.683"",""GVPTot"":16,""VPTot"":17,
""attenAvrWithGVP"":""0.418"",""VPAvr"":""0.204"",""BAPTot"":4,""impulseAvr"":""0.824"",""BAPAvr"":""0.824"",""BPTot"":0,
""missTot"":2,""BPAvr"":0,""impulseTot"":4,""attenTot"":15,""attenAvr"":""0.678"",""attenGrade"":28,""impulseGrade"":60,
""lvlDistType"":""vis1"",""hyperAvr"":0,""hyperGrade"":100,""hyperTot"":0,""hyperTotWithBHV"":1,""attenGradeWitnGVP"":84,
""hyperAvrWithBHV"":""0.683"",""GPTot"":15,""hyperGradeWithBHV"":90,""GPAvr"":""0.678"",""lvlNum"":2,""GVPAvr"":""0.174""},
{""BHPTot"":0,""BHPAvr"":0,""BHVTot"":6,""attenTotWithGVP"":31,""BHVAvr"":""0.949"",""GVPTot"":12,""VPTot"":18,
""attenAvrWithGVP"":""0.417"",""VPAvr"":""0.414"",""BAPTot"":4,""impulseAvr"":""0.659"",""BAPAvr"":""0.659"",""BPTot"":0,
""missTot"":2,""BPAvr"":0,""impulseTot"":4,""attenTot"":19,""attenAvr"":""0.588"",""attenGrade"":44,""impulseGrade"":60,
""lvlDistType"":""vis2"",""hyperAvr"":0,""hyperGrade"":100,""hyperTot"":0,""hyperTotWithBHV"":6,""attenGradeWitnGVP"":84,
""hyperAvrWithBHV"":""0.949"",""GPTot"":19,""hyperGradeWithBHV"":40,""GPAvr"":""0.588"",""lvlNum"":3,""GVPAvr"":""0.146""},
{""BHPTot"":0,""BHPAvr"":0,""BHVTot"":1,""attenTotWithGVP"":30,""BHVAvr"":""0.067"",""GVPTot"":8,""VPTot"":9,
""attenAvrWithGVP"":""0.490"",""VPAvr"":""0.143"",""BAPTot"":0,""impulseAvr"":0,""BAPAvr"":0,""BPTot"":0,""missTot"":3,
""BPAvr"":0,""impulseTot"":0,""attenTot"":22,""attenAvr"":""0.613"",""attenGrade"":56,""impulseGrade"":100,""lvlDistType"":""sound1"",
""hyperAvr"":0,""hyperGrade"":100,""hyperTot"":0,""hyperTotWithBHV"":1,""attenGradeWitnGVP"":76,""hyperAvrWithBHV"":""0.067"",
""GPTot"":22,""hyperGradeWithBHV"":90,""GPAvr"":""0.613"",""lvlNum"":4,""GVPAvr"":""0.152""},{""BHPTot"":1,""BHPAvr"":""2.552"",
""BHVTot"":3,""attenTotWithGVP"":33,""BHVAvr"":""0.602"",""GVPTot"":17,""VPTot"":20,""attenAvrWithGVP"":""0.356"",
""VPAvr"":""0.184"",""BAPTot"":2,""impulseAvr"":""0.535"",""BAPAvr"":""0.535"",""BPTot"":0,""missTot"":0,""BPAvr"":0,
""impulseTot"":2,""attenTot"":16,""attenAvr"":""0.617"",""attenGrade"":32,""impulseGrade"":80,""lvlDistType"":""sound2"",
""hyperAvr"":""2.552"",""hyperGrade"":90,""hyperTot"":1,""hyperTotWithBHV"":4,""attenGradeWitnGVP"":100,""hyperAvrWithBHV"":""1.090"",
""GPTot"":16,""hyperGradeWithBHV"":60,""GPAvr"":""0.617"",""lvlNum"":5,""GVPAvr"":""0.110""},{""BHPTot"":3,""BHPAvr"":""2.480"",
""BHVTot"":5,""attenTotWithGVP"":30,""BHVAvr"":""0.293"",""GVPTot"":12,""VPTot"":17,""attenAvrWithGVP"":""0.447"",""VPAvr"":""0.260"",
""BAPTot"":3,""impulseAvr"":""0.493"",""BAPAvr"":""0.493"",""BPTot"":0,""missTot"":3,""BPAvr"":0,""impulseTot"":3,""attenTot"":18,
""attenAvr"":""0.581"",""attenGrade"":40,""impulseGrade"":70,""lvlDistType"":""both1"",""hyperAvr"":""2.480"",""hyperGrade"":70,
""hyperTot"":3,""hyperTotWithBHV"":8,""attenGradeWitnGVP"":76,""hyperAvrWithBHV"":""1.113"",""GPTot"":18,""hyperGradeWithBHV"":20,
""GPAvr"":""0.581"",""lvlNum"":6,""GVPAvr"":""0.246""},{""BHPTot"":1,""BHPAvr"":""2.212"",""BHVTot"":4,""attenTotWithGVP"":31,
""BHVAvr"":""0.207"",""GVPTot"":9,""VPTot"":13,""attenAvrWithGVP"":""0.491"",""VPAvr"":""0.166"",""BAPTot"":3,
""impulseAvr"":""0.597"",""BAPAvr"":""0.597"",""BPTot"":0,""missTot"":2,""BPAvr"":0,""impulseTot"":3,""attenTot"":22,
""attenAvr"":""0.631"",""attenGrade"":56,""impulseGrade"":70,""lvlDistType"":""both2"",""hyperAvr"":""2.212"",""hyperGrade"":90,
""hyperTot"":1,""hyperTotWithBHV"":5,""attenGradeWitnGVP"":84,""hyperAvrWithBHV"":""0.608"",""GPTot"":22,""hyperGradeWithBHV"":50,
""GPAvr"":""0.631"",""lvlNum"":7,""GVPAvr"":""0.148""},{""BHPTot"":0,""BHPAvr"":0,""BHVTot"":1,""attenTotWithGVP"":30,
""BHVAvr"":""0.410"",""GVPTot"":11,""VPTot"":12,""attenAvrWithGVP"":""0.403"",""VPAvr"":""0.151"",""BAPTot"":4,
""impulseAvr"":""0.422"",""BAPAvr"":""0.422"",""BPTot"":0,""missTot"":3,""BPAvr"":0,""impulseTot"":4,""attenTot"":19,
""attenAvr"":""0.562"",""attenGrade"":44,""impulseGrade"":60,""lvlDistType"":""Basic2"",""hyperAvr"":0,""hyperGrade"":100,
""hyperTot"":0,""hyperTotWithBHV"":1,""attenGradeWitnGVP"":76,""hyperAvrWithBHV"":""0.410"",""GPTot"":19,""hyperGradeWithBHV"":90,
""GPAvr"":""0.562"",""lvlNum"":8,""GVPAvr"":""0.127""}]",
xml_object_clicks:"",test_age:9,zscore_a:0.25022748,zscore_t:1.295495495,zscore_h:0.418705036,zscore_i:1.273542601,modify_user_id:1784513,child_id:"",details_id:"",profile_type:"",focus_table_imported:"",test_age_months:115,treatment_id:2,other_treatment:"",findings:"",summary:"",observer_name:"",record_type:test,tag1:"",tag2:"",tag3:"",tag4:"",moxo_run_date:44:04.9,x:10,t0:1644921860,ott:91d136dbe072bd2dea2d34af90f3bca2,successfull_practice:TRUE,a1:32,a2:31,a3:31,a4:30,a5:33,a6:31,a7:30,a8:22,t1:15,t2:19,t3:22,t4:16,t5:18,t6:22,t7:19,t8:3,h1:1,h2:6,h3:1,h4:4,h5:8,h6:5,h7:1,h8:1,i1:4,i2:4,i3:0,i4:2,i5:3,i6:3,i7:4,i8:0,medication_name:None,doctor_name:"",patient_name:"",testordinal:1,testcount:1,test_tag:Test,gender:M,signed_zscore_a:-0.25022748,signed_zscore_t:-1.295495495,signed_zscore_h:-0.418705036,signed_zscore_i:-1.273542601,country_for_norms:8,tagging_type:""
}

## BackLog
1. Get a copy of structure of DataBase with a little of data as example.
2. Improving computing of current paramtres as microsevice on Python/Flask (BlackBox): creating endpoint with analytics and filling relevant tables on database. _By this we take out computing process from NodeJS code_
3. Improving R-models to current BlackBox (for computing more parameters).
4. Developing FrontEnd and PDF-reports for new elements of knowledge. 
5. Implamentation endpoints for autonomus service (get request/give responds).
6. Implamentation endpoints to architecture of NodeJS-back end (for realtime analytics).


1. Делаем прорект разработки (как все будет выглядеть и взаимодействовать) Для этого получаем копию структурв БД и тестовый набор данных как пример. А также код NodeJs. (Идеальный вариант - развернуть на dev-сервере) Для того, чтобы разобраться со струкутной данных и разобраться с архитектрурой NodeJS.
2. Реализуем на Python функциональность, которая на данный момент реализуется на NodeJS (существующие 4 параметра для отчета). Этим мы дублируем существующую функциональность на NodeJS. Для того, чтобы поднять отдельный проецесс на Python, который работает с той же БД, но получает запрос на вычисления от NodeJS.
3. Внедряем разработанные на R модели для работы с данными (через использование моделей R в Python или переписванию моделей R на Python). _Оставляем R для экспериментов и работы с данными, но в реализации - это может быть переход на Python полностью или realtime-взаимодействие Python-R._
4. Разрабатываем интерфейс и дополнение к PDF-отчету для работы с новыми знаниями (берутся из новых таблиц БД).
5. Реализуем эндпоинты для автономной работы сервиса.
6. Внедряем взаимодействие с внешним сервисом в существующее приложение.

**Вопросы:**
1. Какой алгоритм считает первичные коэффиценты (делает препроцессинг)? 
2. Мы как-то трогаем алгоритм препроцессинга?
3. Какие именно процессы вычисления защищены авторским правом (принадлежат не нам)?
4. Какие есть интерфейсы в основном приложении (ребенок/доктор)?