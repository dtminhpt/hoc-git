links:
1.http://www.testingtools.com/test-automation/
2. TDD:
http://www.agiledata.org/essays/tdd.html
3. agile blog:
http://agiletesting.blogspot.com/2005/02/performance-vs-load-vs-stress-testing.html



——


1.4	PHAM VI TEST : Các giai đoạn kiểm tra được thực hiện : (Khái quát định nghĩa từng mức độ trong các giai đoạn , thành viên cần phải nắm rõ để biết được quy trình kiểm tra phần mềm Website Đoàn trường THPT Nguyễn Du sẽ được diễn ra như thế nào )
@@@@@•	Unit Test – kiểm thử mức đơn vịo	Mục đích của Unit Test là bảo đảm thông tin được xử lý và xuất (khỏi Unit) là chính xác, trong mối tương quan với dữ liệu nhập và chức năng của từng đơn vị thành phần nhỏ nhất của phần mềmo	Kiểm tra từng đơn vị thành phần nhỏ nhất của Website Đoàn trường THPT Nguyễn Du gồm : các hàm (Function), thủ tục (Procedure), lớp (Class), hoặc các phương thức (Method)o	Một kinh nghiệm đúc kết từ thực tiễn: thời gian tốn cho Unit Test sẽ được đền bù bằng việc tiết kiệm rất nhiều thời gian và chi phí cho việc kiểm thử và sửa lỗi ở các mức kiểm thử sau đó do đó chúng ta sẽ cố gắng thực hiện Unit Test thật tốto	Vì Unit Test thường thường do lập trình viên thực hiện trong giai đoạn viết code và xuyên suốt chu kỳ phát triển phần mềm. Do đó, Unit Test đòi hỏi kiểm thử viên có kiến thức về thiết kế và code của chương trìnho	Unit Test cũng đòi hỏi phải chuẩn bị trước các tình huống (test case) hoặc kịch bản (script), trong đó chỉ định rõ dữ liệu vào, các bước thực hiện và dữ liệu mong chờ sẽ xuất ra. Các test case và script này nên được giữ lại để tái sử dụng@@@@@@•	Integration Test – kiểm thử tích hợpo	Integration test kết hợp các thành phần của một ứng dụng và kiểm thử như một ứng dụng đã hoàn thành. o	Integration Test có 2 mục tiêu chính:•	Phát hiện lỗi giao tiếp xảy ra giữa các Unit•	Tích hợp các Unit đơn lẻ thành các hệ thống nhỏ (subsystem) và cuối cùng là nguyên hệ thống hoàn chỉnh (system) chuẩn bị cho kiểm thử ở mức hệ thống (System Test)o	Integration Test chỉ nên thực hiện trên những Unit đã được kiểm tra cẩn thận trước đó bằng Unit Test, và tất cả các lỗi mức Unit đã được sửa chữao	Có 4 loại kiểm thử trong Integration Test:•	Kiểm thử cấu trúc (Structure Test): Tương tự White Box Test •	Kiểm thử chức năng (Functional Test): Tương tự Black Box Test •	Kiểm thử hiệu năng (Performance Test): kiểm thử việc vận hành của hệ thống•	Kiểm thử khả năng chịu tải (Stress Test): kiểm thử các giới hạn của hệ thống@@@@@@@•	System Test - kiểm thử mức hệ thống o	Mục đích System Test là kiểm thử thiết kế và toàn bộ hệ thống (sau khi tích hợp) có thỏa mãn yêu cầu đặt ra hay khôngo	System Test .bắt đầu ngay sau Integration Test,trọng tâm là đánh giá về hoạt động, thao tác, sự tin cậy và các yêu cầu khác liên quan đến chất lượng của toàn hệ thốngo	Điểm khác nhau then chốt giữa Integration Test và System Test là System Test chú trọng các hành vi và lỗi trên toàn hệ thống, còn Integration Test chú trọng sự giao tiếp giữa các đơn thể hoặc đối tượng khi chúng làm việc cùng nhauo	Bản thân System Test lại gồm nhiều loại kiểm thử khác nhau ,phổ biến nhất gồm:•	Kiểm thử chức năng (Functional Test)•	Kiểm thử khả năng vận hành (Performance Test)•	Kiểm thử khả năng chịu tải (Stress Test hay Load Test)•	Kiểm thử cấu hình (Configuration Test)•	Kiểm thử khả năng bảo mật (Security Test)•	Kiểm thử khả năng phục hồi (Recovery Test)o	Nhìn từ quan điểm người dùng, các cấp độ kiểm thử trên rất quan trọng: bảo đảm hệ thống đủ khả năng làm việc trong môi trường thựco	Lưu ý không nhất thiết phải thực hiện tất cả các loại kiểm thử nêu trên. Tùy yêu cầu và đặc trưng của từng hệ thống, tuỳ khả năng và thời gian cho phép của dự án, khi lập kế hoạch, người Quản lý dự án sẽ quyết định áp dụng những loại kiểm thử nào. Chính vì thế , đối với Website Đoàn trường THPT Nguyễn Du chúng ta sẽ kiểm thử những chức năng thiết yếu nhất đối với 1 Website : chức năng, chịu tải, vận hành và bảo mật@@@@@@•	Acceptance Test - kiểm thử chấp nhận sản phẩmo	Thông thường, sau giai đoạn System Test là Acceptance Test, được khách hàng thực hiện (hoặc ủy quyền cho một nhóm thứ ba thực hiện). Mục đích của Acceptance Test là để chứng minh PM thỏa mãn tất cả yêu cầu của khách hàng và khách hàng chấp nhận sản phẩm (và trả tiền thanh toán hợp đồng)o	Acceptance Test có ý nghĩa hết sức quan trọng, mặc dù trong hầu hết mọi trường hợp, các phép kiểm thử của System Test và Accepatnce Test gần như tương tự, nhưng bản chất và cách thức thực hiện lại rất khác biệtViệc kiểm tra Website Đoàn trường THPT Nguyễn Du được thực hiện lần đầu tiên từ lúc hiện thực đến khi hoàn thành, chính vì thế Group 7 sẽ phải test tất cả chức năng hiện có của phần mềm này, bao gồm :




—

1. SUPPORTING TOOLS: xcode, genymotion


2. RECORD TESTS:
SMARTBEAR:
https://support.smartbear.com/viewarticle/70284/


3. AUTOMATIC TESTS:
Notes: Can xem them ngon ngu lap trinh 


4. Web Test

——————————————————————————————————————Terms: 
test case 

qa documents 
test scenarios 

expected results 
data sets 

test procedure 

scripts 

applicable testing tools 
——
KICHOFFS


QA KICKOFFS

NO MORE DOTING 

REVIEW

ALL TESTING DONE BY DEVS 

TAKEAWAY

SOFTWARE 


WEB PRODUCTS

CREATE TEST PLAN 

TEST REPORT 

TEST REPORT 

TEST PLAN 

TEST CASE 

EXECUTE TEST CASE 

AUTOMATION TEST 

TRACK BUGS 

REPORT TO PROJECT MANAGER 

REPORT TO BSE MANAGER 

COMMUNICATE DIRECTLY WITH CUSTOMER ON THE REQUIREMENTS 

WORK CLOSELY WITH THE DEVS
2 YEARS EXPERIENCE AS A WEB TESTER 

TECHNICAL KNOWLEDGE 

WEB DEVELOPMENT METHDOLOGIES 

DESIGN 

IMPLEMENTATION 

DOCUMENTING TEST CASES 

BUGS 

ASSOCIATED REPORTING 

PERFORMANCE TESTING 
WILL BE DONE BY CLIENT 
PERFORMANCE TESTING - CLIENT 

STRESS TESTING 
STRESS TESTING 
STRESS TESTING 
STRESS TESTING - CLIENT 
STRESS TESTING - CLIENT 

SECURITY AND ACCESS CONTROL TESTING 
SECURITY AND ACCESS CONTROL TESTING 
SECURITY AND ACCESS CONTROL TESTING - CLIENT 
CLIENT : TEST BAO MAT 
CLIENT : TEST BAO MAT 

USER ACCEPTANCE TESTING 
CONFORM = TUAN THEO 
CONFORM = TUAN THEO 

USER ACCEPTANCE TESTING 
USER ACCEPTANCE TESTING 
USER ACCEPTANCE TESTING 



READY FOR OPERATIONAL USE 
READY FOR OPERATIONAL USE 
READY FOR OPERATIONAL USE 
RESDY FOR OPERARIONAL USE 

ACCEPTANCE TESTIGN 
USER ACCEPTANCE TESTING 

USER ACCEPTANCE TESTING - CLIENT 
- CLIENT 


ALPHA TESTING 
ALPHA TESTING 
ALPHA TESTING 

BETA TESTING 
BETA TESTING 
BETA TESTING 

ALPHA TESTING 
ALPHA TESTING 
ALPHA TESTING 
ALPHA TESTING 

CONDUCT 
CONDUCT - CLIENT 
CONDUCT - CLIENT 
CONDUCT - CLIENT 


DEVELOPER’S SITE BY CLIENT 
DEVELOPER’S SITE BY CLIENT 

DEVELPER’S SITE BY CLIENT 
DEVEOPER’S SITE BY CLIENT 

DEVELOPER’S SITE BY CLIENT 


test schedule

test schedule

test schedule

high-level test planning 
hing-level test planning 

master qa plan 
master qa plan 

master qa plan 


qa schedule 
qa schedule 

qa schedule 

milestone = giai doan 
milstone = giai doan 
milestone = giai doan 

the high level planning 

the high level planning 

deliverables 
deliverables 

project plan 
project plan 
prject plan 
project plan 

program function specifications 

program function specifications 

program function specifications 


design phase 

cong suc nhieu but 

cong suc nhieu 




design phase 
design phase 
design phase 


test engineer
test engineer 
test engineer 
test engineer 

inspect = kiem tra ki 
inspect = kiem tra ki 
inspect = kiem tra ki 

review the requirement 
review the requirement 

design documents 
design documents 

design documents 
design documents are completed 
are completed 

test engineers 
test engineers 

encouraged 
are encouraged
are encouraged 

to start working on the Test Plan document 
to start working on the Test Plan document 

test design planning 
test design planning 


Code Complete 
Code Complete 

Infrastructure 
Infrastructure



Test enginner
Test engineers 
Test engineers

in the final stages 
in the final stages 
prelinary 
preliminary infrastructure 

Test Plan 
Test Plan 

test cases 
test cases

other QA documents 

test execution 










QA documents 

Test Plan 
Test Plan 
Test Plan 
test cases 
test cases 

QA documents 
QA documents 

QA documents



test execution for each feature 
test execution for each feature 
test execution for each feature 

test scenarios
test scenarios 
test scenarios 
test scenarios 

expected results
expected results
expected results 

data sets 
data sets 
data sets 

test procedures
test procedures 
test procedures 

scripts - automation test 
scripts - automation test 
scripts - automation test 

scripts

applicabel testing tools 
applicable testig tools

applicable testing tools 










feature complete 
khong nen hoc thuoc long 
should not lear by heart




feature complete 

ghi chi can than 
ghi chu can than 

feature complete


QA documentation 

QA documentation 

test engineers 
test engineers 


assess = danh gia 
assess = danh gia 
assess = danh gia 
assess = danh gia 

Binary tree feature 
binary tree feature 
binary tree feature 

test scenarios
test scenarios 

expected results
expected results
expected results

data sets 
data sets 
data sets 
data sets 
data sets 
data sets 

test procedure 
test procedure 
test procedure 
test procedure 

script
script
aplicable testing tools 
applicable testing tools 

applicable testing tools 



beta regression 
beta regression 
beta regression 
beta regression 

beta shutdown 
beta shutdown 
beta shutdown 


ship/live 
ship/live 

ship/live 



unfinished testing documents
unfinished testing documents 
unfinished testing documents



control procedure 
control  procedure 
control procedure 

review 
review 
following documents 

following documents 

review report 

review report 

will be prepare 






will be prepare for each work products 

will be prepare for each work products 


test cases 
test cases

test cases 


RTM = Requirement Traceability Matrix = ma tran theo vet nhung yeu cau 

Requirement Traceability Matrix 

Requirement Traceability Matrix

= Ma tran kha nang theo vet nhung yeu cau 








Requirement Traceability Matrix 

Requirement Traceability Matrix
Requirement Traceability Matrix 

bugs review meetings

bug review testings
will be held
for every test cycle 

be held for evey test cycle 
be held for evey test cycle 
be held for evey test cycle 

conduct during the following 


GUI testing 
GUI testing 
GUI testing 

Report Output/Data Testing 
Report Output / Data Testing 


critical 
critical 

show stoppers 
bugs 
show stoppers bugs 

Chan


change request 
change request for report

change request for report 
change reques for report 

change request for report 


using following process
using following process
change request 

change request -> its impact on existing report functionality
high priority 

change request -> its impact on existing report functionality 

change request -> its impact on existing report functionality 


if the change is major, test cases will be updated 
if the change is major, test cases will be updated 
if the change is major, test cases will be updated 

if the change is major, the test cases will be updated 

if the change is minor, tst cases will may not be updated 
if the chaneg is minor, test cases will may not be updated 
if the change is minor, test cases will may not be updated 

retesting and regression testing will be done as per changed request 
retesting and regression testing will be done as per changed request 

retesting and regression testing will be done per changed request 




retesting and regression testing 
retesting and regression testing will be done as per changed request

retesting and regression testing will be done as per changed request 

retesting and regression testing will be done as per changed request 



defect reporting 
defect reporting 

static testing 
static testing 
static testign 
dynamic testing 
dynamic testing 
bugzilla
bugzilla bug tracking tool 
bugzilla bug tracking tool 
bugzilla bug tracking tool 






roles and responsibilities 

roles and responsibilities 
roles and responsibilities 

roles and responsibilities 




role
responsibilities 
role
responsibilities 

pm = project manager 
pm = projet manager 

qa team 
qa team 
qa team 

project schedule 
project schedule 
project schedule 

the overll success of the project 
the overall success of he project 

QA
qa 
understand requirements
understand requirements 

writing and executing test cases 
writing and executing test cases 



preparing RTM 
rtm 
rtm 

reviewing test cases , rtm 
reviwing test cases, rtm 


defect reporting snd trakign 
defect reporting and tracking 
defect reporting and tracking 
defect reporting and tracking 



defect reporting and tracking 
defect reporting and tracking 
defect reporting and tracking 

retesting and regression testing 
retesting and regression testing 
retesting and regression testing 


bug review meeting 
bug review meeting 


deliverable 
deliverable  

test design document test plan document 
test design document test plan document 
test design document 
test plan document 
test plan document 
test plan document 
unit white-box test design 
unit white-box test design 
white-box test design 

white testing criteria 
white testing criteria 

methods 
methods 
test cases 
test case 

system test design 
system test design 

unit 
unit 
system 
system 
system 

system test criteria
system test criteria 

methods
methods 
test cases 
test cases 
scripts
scripts
scripts



unit black-box test design 
unit black-box tet design 
uit black-box test design 

black-box testing criteria 
black-box testing criteria

black-box testing criteria 


test report document 
test report document 
test report document 

system test report 
system test report 
system test report 

system test result
system test result 
entry criteria 
entry criteria 
entry criteria 

source code 

source code 

source code 
source code 

unit tested
unit tested 

unit tested 

bw in place
be inplace 
be in place 

qa completely undersood the requirements 

qa completely understooa the requirements
qa completely understood the requirements
qa completely understood the requirements

reviewed test scenarios
reviewed test scenarios
reviewed test scenarios, test cases and rt
reviewed test scenarios, test cases and rtm 


suspension criteria 
suspension criteria 
suspension criteria 

serious defects 
serious defects 
serious defects 

the build contains many serious defects which seriously or limit testing prgress
suspension criteria 
suspension criteria

suspension criteria 

suspension criteria 
suspension criteria 

the build
the build 
the build 

serious defects 
serious defects 
serious defects 

limit testing progress 
limit testing progress 
limit testing progress

significant change 
significant change 
significant change 

in requirements suggested by client 
in requirement suggested by client 
i requirement suggested by clent 

software/hardware problems 
software/hardware problems 
software/hardware problems 

assigned resources 
assigned resources 
assigned resources 

assigned resources 

assigned resources 

assigned resources 

assigned resources 
assigned resources 
assigned resouces 

assigned resources 

asigned resources 

assigned resources 

assigned resources are not available when needed by test team 
assigned resources are not available when needed by test team 
assigned resources are not available when needed by test team 


resumption criteria 
resumption criteria 
resumpton criteria 

resumption will only occur when the problem that caused the caused the suspension 

have been resolved 

resumption will only occur when the problem that caused the suspension have been resolved 


exit criteria 
exit criteria 
exit criteria 

exit criteria 

no defects over a period of time or less testing efforts 

no defects over a period of time or less testing efforts

no defects over a period of time or less testing effort 

all the high priority/ severity test cases has been executed 

all the high priority/ severity test cases has been executed 

all the high priority/ severity test cases has been executed 

all the high priority/ severity test cases has been executed 



deliverables are ready 

deliverables are ready 

deliverables are ready 
deliverables are ready 


high severity/priority bugs are fixed 

high severity/ priority bugs are fixed 


risk 

delay in delivery of test items might require increases night shift 

delay in delivry of test itesm require increased night shift scheduling to meet the delivery date 


delay in delivery of test items might require increased night shift scheduling to meet the delivery date 

delay in delivery of test itesm might require increased night shift scheduling to meet the delivery date \\


delay in delivery of test items might require increased night shift scheduling to meet the delivery date 

understanding requirements
inderstanding requirements 

understanding requirements 

understanding the requirements 

domain and project knowledge 
domain and project knowledge 


domain and project knowledge 
domain and project knowledge 

acronyms
acronyms
acronyms
acronyms


GUI 
rtm = requirement traceability matrix 
requirement traceability matrix 
rtm = requirement traceability matrix 
requirement traceability matrix 
requirement traceability matrix 

requirement traceability matrix
requirement traceability matrix 
requirement traceability matrix 

software testing folks 

software testing tutorial 

software testing tutorial 

testing article 

selenium is a popular automated web testing tool 
a popular automated web testing tool 
a popular automated web testing tool 


