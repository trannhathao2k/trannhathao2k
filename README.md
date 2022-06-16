# Báo cáo thực tập



- [1. Spring Framework](#1-spring-framework)
  - [1.1. Các module và kiến trúc của Spring Framework](#11-các-module-và-kiến-trúc-của-spring-framework)
  - [1.2. Spring Boot](#12-spring-boot)
- [2. Angular](#2-angular)
- [3. So sánh Cơ sở dữ liệu quan hệ và Cơ sở dữ liệu NoSQL](#3-so-sánh-cơ-sở-dữ-liệu-quan-hệ-và-cơ-sở-dữ-liệu-nosql)
- [4. Microservices](#4-microservices)
  - [4.1. Phân biệt giữa kiến trúc nguyên khối và kiến trúc Microservices](#41-phân-biệt-giữa-kiến-trúc-nguyên-khối-và-kiến-trúc-microservices)
    - [4.1.1. Kiến trúc nguyên khối](#411-kiến-trúc-nguyên-khối)
    - [4.1.2. Kiến trúc Microservices](#412-kiến-trúc-microservices)
    - [4.1.3. Ưu nhược điểm của kiến trúc Microservices](#413-ưu-nhược-điểm-của-kiến-trúc-microservices)
- [5. Giới thiệu về TypeScript](#5-giới-thiệu-về-typescript)
- [6. Sơ đồ mô tả](#6-sơ-đồ-mô-tả)
  - [6.1. Sơ đồ Use case tổng quát](#61-sơ-đồ-use-case-tổng-quát)
  - [6.2. Sơ đồ Use case Quản lý danh mục](#62-sơ-đồ-use-case-quản-lý-danh-mục)
  - [6.3. Sơ đồ lớp](#63-sơ-đồ-lớp)
  - [6.4. Sơ đồ tuần tự](#64-sơ-đồ-tuần-tự)
    - [6.4.1. Sơ đồ tuần tự Quản lý danh mục](#641-sơ-đồ-tuần-tự-quản-lý-danh-mục)
    - [6.4.2. Sơ đồ tuần tự Nhập xuất kho NCC](#642-sơ-đồ-tuần-tự-nhập-xuất-kho-ncc)
    - [6.4.3. Sơ đồ tuần tự Chuyển kho](#643-sơ-đồ-tuần-tự-chuyển-kho)
    - [6.4.4. Sơ đồ tuần tự Tra cứu tồn kho](#644-sơ-đồ-tuần-tự-tra-cứu-tồn-kho)
    - [6.4.5. Sơ đồ tuần tự Tra cứu thông tin chuyển kho](#645-sơ-đồ-tuần-tự-tra-cứu-thông-tin-chuyển-kho)
- [7. Công cụ Jhipster](#7-công-cụ-jhipster)
  - [7.1. Client side](#71-client-side)
  - [7.2. Server side](#72-server-side)
  - [7.3. Deployment](#73-deployment)
- [8. Ứng Dụng Angular trong Jhipster](#8-ứng-dụng-angular-trong-jhipster)
  - [8.1. Cấu trúc dự án](#81-cấu-trúc-dự-án)
  - [8.2. i18n](#82-i18n)
  <div style="page-break-after: always;"></div>

### 1. Spring Framework

Spring Framework là mô hình lập trình và cấu hình cho các ứng dụng doanh nghiệp dựa trên Java, Spring có thể được sử dụng để phát triển Java Desktop, ứng dụng mobile, Java Web.

#### 1.1. Các module và kiến trúc của Spring Framework

**Test:** Đây là tầng cung cấp cho người dùng khả năng hỗ trợ kiểm thử với JUnit và TestNG. Module cung cấp các đối tượng mà bạn có thể dùng để kiểm tra.
**Spring Core Container:** Nó có bao gồm một số module như:
- Spring-core, Spring-bean: Có khả năng cung cấp các tính năng như: IOC và Dependency Injection. 
- Spring-context: Hỗ trợ các dạng đa ngôn ngữ và các tính năng Java EE cho người dùng như: EJB, JMX.
- Spring-expression: Có khả năng mở rộng từ Expresion Language bên trong JSP. Từ đó, cung cấp các hỗ trợ cho quá trình setting hoặc getting các giá trị. Hầu hết các method đều sẽ thực hiện cải tiến cho phép truy cập vào collections, index, các toán tử logic…
  
**AOP, Aspects and Instrumentation:** 
Spring-aop module này sẽ giữ nhiệm vụ hỗ trợ cho các cài đặt lập trình thiên hướng khía cạnh và khả năng hỗ trợ tích hợp với AspectJ.
Spring-aspects là module riêng biệt cung cấp tích hợp với AspectJ.
Spring-instrument là module cung cấp hỗ trợ thiết bị đo lớp và triển khai trình nạp lớp để được sử dụng trong một số máy chủ ứng dụng nhất định.
**Data Access / Integration:** Đây là nhóm bao gồm JDBC, ORM, OXM, JMS và module Transaction. Chúng có khả năng cung cấp giao tiếp cùng với database.
**Web:** đây là một trong những nhóm bao gồm: Web, Web-Servlet… Nó sẽ hỗ trợ cho việc tạo ra các ứng dụng web.
 
#### 1.2. Spring Boot

Spring Boot là một Spring framework hiện đang được nhiều lập trình viên lựa chọn vì nó giúp cho các lập trình viên chúng ta đơn giản hóa quá trình lập trình một ứng dụng với Spring, chỉ tập trung vào việc phát triển cho ứng dụng.
Spring Boot được dùng để tạo các dự án Spring:
- Giúp xây dựng ứng dụng Spring bao gồm gần như mọi thứ REST API, WebSocket, Web,…
- Giúp giảm tối ưu công đoạn cấu hình và không yêu cầu cấu hình thông qua XML.
- Tích hợp các loại module khác nhau trong các loại Spring như Spring Data, Spring MVC, Spring Security, Spring JDBC, Spring ORM…
- Các starter dependency làm cho việc thêm các hỗ trợ phù hợp cho project giúp cấu hình ban đầu nhanh hơn.
- Bạn có thể dễ dàng phát triển các ứng dụng Spring dựa trên ngôn ngữ Java.
- Spring Boot có thể tự động cấu hình Spring mỗi khi cần thiết.
- Hỗ trợ nhiều IDE như Spring Tool Suite, IntelliJ IDEA, NetBeans hoặc cũng có thể cấu hình đơn giản và dùng Sublime Text để phát triển luôn.
- Không sinh code cấu hình và không yêu cầu phải cấu hình bằng XML …

### 2. Angular

Angular là một javascript framework do google phát triển để xây dựng các Single Page Application (SPA) bằng JavaScript , HTML và TypeScript . Angular cung cấp các tính năng tích hợp cho animation , http service và có các tính năng như auto-complete , navigation , toolbar , menus ,… Code được viết bằng TypeScript , biên dịch thành JavaScript và hiển thị tương tự trong trình duyệt.

**Components**
Components là các khối xây dựng tạo nên một ứng dụng. Một componentsbao gồm một class TypeScript , HTML và styles. 
  - **selector:** Là tên được đặt để gọi một component trong code html.
  - **template:** Là tự định nghĩa khung html cho component .
  - **templateUrl:** Là đường dẫn url tới file html bên ngoài để load file đó vào làm khung html cho component này.
  - **styles:** Là viết style css luôn vào file component này. Cách này chỉ dùng cho component đơn giản.
  - **styleUrls:** Là đường dẫn url đến file style css độc lập cho component này.


### 3. So sánh Cơ sở dữ liệu quan hệ và Cơ sở dữ liệu NoSQL

|                 | Cơ sở dữ liệu quan hệ                                                                                                                                                                                                                                                         | Cơ sở dữ liệu NoSQL                                                                                                                                                                                                                                                                                                                                                                                              |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Mô hình dữ liệu | Mô hình quan hệ chuẩn hóa dữ liệu vào bảng được hình thành từ hàng và cột. Sơ đồ quy định rõ ràng bảng, hàng, cột, chỉ mục, mối quan hệ giữa các bảng và các thành tố cơ sở dữ liệu khác. Cơ sở dữ liệu sẽ thực thi tính toàn vẹn tham chiếu trong mối quan hệ giữa các bảng. | Các cơ sở dữ liệu NoSQL cung cấp nhiều mô hình dữ liệu khác nhau như khóa-giá trị, tài liệu và biểu đồ, được tối ưu hóa để đạt hiệu năng và quy mô tối ưu.                                                                                                                                                                                                                                                        |
| Thuộc tính ACID | Cơ sở dữ liệu quan hệ có các thuộc tính mang tính nguyên tố, nhất quán, tách biệt và bền vững (ACID)                                                                                                                                                                          | Cơ sở dữ liệu NoSQL thường phải đánh đổi bằng cách nới lỏng một số thuộc tính ACID này của cơ sở dữ liệu quan hệ để có mô hình dữ liệu linh hoạt hơn có khả năng thay đổi quy mô theo chiều ngang. Việc này biến các cơ sở dữ liệu NoSQL thành lựa chọn tuyệt vời cho các trường hợp sử dụng cần thông lượng cao, độ trễ thấp cần thay đổi quy mô theo chiều ngang vượt qua giới hạn của một phiên bản duy nhất. |
| Hiệu năng       | Hiệu năng thường phụ thuộc vào hệ thống con của ổ đĩa. Thông thường, việc tối ưu hóa các truy vấn, chỉ mục và cấu trúc bảng bắt buộc phải được thực hiện để đạt mức hiệu năng tối đa.                                                                                         | Hiệu năng thường được xem là chức năng của kích cỡ cụm phần cứng ngầm, độ trễ mạng và ứng dụng đưa ra lệnh gọi.                                                                                                                                                                                                                                                                                                  |
| Quy mô          | Cơ sở dữ liệu quan hệ thường tăng quy mô bằng cách tăng năng lực điện toán của phần cứng hoặc tăng quy mô bằng cách thêm bản sao của khối lượng công việc chỉ đọc.                                                                                                            | Cơ sở dữ liệu NoSQL thường có tính phân mảnh cao do các mẫu truy cập khóa-giá trị có khả năng tăng quy mô bằng cách sử dụng kiến trúc được phân phối để tăng thông lượng, đem đến hiệu năng ổn định với quy mô gần như không giới hạn.                                                                                                                                                                           |
| API             | Yêu cầu lưu trữ và truy xuất dữ liệu được truyền đạt bằng cách sử dụng các truy vấn nhất quán với ngôn ngữ truy vấn có cấu trúc (SQL). Các truy vấn này được phân tích và thực thi bởi cơ sở dữ liệu quan hệ.                                                                 | API trên cơ sở đối tượng cho phép các nhà phát triển ứng dụng dễ dàng lưu trữ và truy xuất cấu trúc dữ liệu trong bộ nhớ. Khóa phân mảnh tìm kiếm các cặp khóa-giá trị, tập hợp cột hoặc văn bản có cấu trúc chưa hoàn chỉnh có chứa đối tượng và thuộc tính của ứng dụng được xếp theo chuỗi.                                                                                                            |

### 4. Microservices
#### 4.1. Phân biệt giữa kiến trúc nguyên khối và kiến trúc Microservices
##### 4.1.1. Kiến trúc nguyên khối
Người lập trình xây dựng hệ thống chỉ trong một khối cung cấp các tính năng đáp ứng nhu cầu của người sử dụng. Khi hệ thống đưa vào sử dụng, và thành công của hệ thống sẽ thu hút nhiều người sử dụng, từ đó, nhu cầu về tính năng mới của hệ thống sẽ tăng cao. Khi phải thêm nhiều tính năng mới vào hệ thống, dữ liệu sẽ tăng lên, dẫn đến hệ thống sẽ càng ngày càng phức tạp, việc bảo trỉ, nâng cấp cho hệ thống cũng sẽ gặp rất nhiều khó khăn, thậm chí là không thể, hoặc chi phí bỏ ra để xây dựng hệ thống khác sẽ ít hơn chi phí sửa chữa cho hệ thống cũ. Khi hệ thống càng lớn, mỗi lần cho ra phiên bản mới cũng sẽ rất khó khăn, có thể làm trễ tiến độ của người sử dụng. Ngoài ra, hệ thống lớn sẽ ảnh hưởng đến khả năng làm việc của các lập trình viên tham gia phát triển hệ thống.

##### 4.1.2. Kiến trúc Microservices

- Để giải quyết những vấn đề của kiến trúc nguyên khối, ý tưởng được đề xuất là chia nhỏ hệ thống lớn ra thành những dịch vụ nhỏ kết nối với nhau. Mỗi dịch vụ nhỏ thực hiện một tập các chức năng chuyên biệt như quản lý đơn hàng, quản lý khách hàng,…Mỗi dịch vụ là một ứng dụng nhỏ kết nối thông qua bộ chuyển đổi (Adapter) khác nhau. Một số dịch vụ có nhiệm vụ làm API cho phép giao tiếp với các dịch vụ nhỏ khác hay các ứng dụng khác gọi tới. Khi vận hành, mỗi dịch vụ nhỏ được chạy trong một máy ảo (Virtual Machine) hoặc Docker Container (ảo hóa tầng ứng dụng).
- Như vậy, mỗi vùng chức năng giờ đã được thực thi bởi một dịch vụ nhỏ, ứng dụng web cũng có thể chia nhỏ hơn cho từng nhóm đối tượng người dùng (quản lý, khách hàng,..). Thiết kế giao diện cho từng nhóm đối tượng người dùng giúp tối ưu hóa trải nghiệm, tốc độ nhanh hơn, dễ tương thích hơn trong khi cấu trúc chức năng đơn giản hơn.
- Kiến trúc microservices chú trọng nhiều đến quan hệ giữa ứng dụng và CSDL. Thay vì dùng chung một cơ sở dữ liệu giữa các dịch vụ, mỗi dịch vụ sẽ có CSDL riêng. Cách này khác so với cơ sở dữ liệu tập trung (Toàn bộ ứng dụng sử dụng chung một CSDL thống nhất). Hệ quả là sẽ có sự dư thừa dữ liệu, cơ chế ràng buộc khóa ngoại cho quan hệ dữ liệu không thể áp dụng với bảng ở 2 cơ sở dữ liệu tách biệt.

##### 4.1.3. Ưu nhược điểm của kiến trúc Microservices

**Ưu điểm của kiến trúc Microservices**

- Đơn giản hóa hệ thống lớn: Vì hệ thống được phân chia ra thành nhiều dịch vụ nhỏ hơn giao tiếp với nhau nên hệ thống lớn sẽ giảm sự phức tạp của hệ thống đi rất nhiều.
- Chia nhỏ ứng dụng một khối cồng kềnh thành các dịch vụ nhỏ dễ quản lý, bảo trì nâng cấp, tự do chọn, nâng cấp công nghệ mới: Hệ thống được chia ra thành nhiều dịch vụ nhỏ hơn nên khi xảy ra lỗi ở một chức năng nào đó trong hệ thống, chỉ cần tìm đến dịch vụ thực hiện chức năng đó để bảo trì sửa chữa, tương tự quá trình nâng cấp, phát triển hệ thống cũng sẽ đơn giản hơn rất nhiều.
- Microservices thúc đẩy tách rạch ròi các khối chức năng : Điều rất khó thực hiện với ứng dụng một khối. Nếu muốn tạo sự rạch ròi trong ứng dụng một khối, sẽ phải thiết kế theo mô hình kiến trúc đặc biệt và phải liên tục tái cấu trúc hệ thống.
- Mỗi dịch vụ nhỏ sẽ phát triển dễ hơn, nhanh hơn, dễ viết mã kiểm thử tự động cho từng dịch vụ nhỏ, điều mà kiến trúc nguyên khối có thể gặp khó khăn.
- Một số dịch vụ nhỏ có thuê ngoài phát triển mà vẫn bảo mật hệ thống và mã nguồn phần dịch vụ còn lại. Đội phát triển có nhiều lựa chọn công nghệ mới, khung phần mềm (framework), CSDL mới, đa dạng để nâng cấp từng dịch vụ nhỏ, chọn môi trường tối ưu nhất để chạy. Các dịch vụ có thể bật tắt để kiểm nghiệm so sánh, tăng tốc quá trình cải tiến giao diện. Việc triển khai phần mềm đều đặn khả thi với Microservices. Dịch vụ nhỏ đóng gói có thể chuyển từ môi trường phát triển sang môi trường chạy thật không phải cấu hình thủ công lại, không phải copy tập tin quá lớn.

**Nhược điểm của Microservices**

- Nhược điểm đầu tiên của Microservices là Microservices nhấn mạnh kích thước nhỏ gọn của dịch vụ. Chia quá nhiều sẽ dẫn đến rời rạc, vụn vặt, khó kiểm soát. Việc lưu dữ liệu cục bộ bên trong những dịch vụ quá nhỏ sẽ khiến dữ liệu phân tán quá mức cần thiết.
- Do hệ thống được chia thành những dịch vụ nhỏ nên phải xử lý sự cố khi kết nối chậm, lỗi khi thông điệp không gửi được hoặc thông điệp gửi đến nhiều đích đến vào các thời điểm khác nhau.
- Đảm bảo giao dịch phân tán cập nhật dữ liệu đúng đắn vào nhiều dịch vụ nhỏ khác nhau rất khó, đôi khi là không thể so với đảm bảo giao dịch cập nhật vào nhiều bảng trong một cơ sở dữ liệu trung tâm.
Kiểm thử tự động một dịch vụ trong kiến trúc Microservices đôi khi yêu cầu phải chạy cả các dịch vụ nhỏ khác mà nó phụ thuộc. Do đó khi phân rã ứng dụng một khối thành Microservices cần luôn kiểm tra mức độ ràng buộc giữa các dịch vụ một cách cẩn thận.
- Nếu các dịch vụ nhỏ thiết kế phục thuộc vào nhau theo chuỗi công việc A gọi B, B gọi C, C gọi D. Nếu một mắt xích có giao tiếp API thay đổi, các mắc xích khác có thể sẽ bị ảnh hưởng. Vì vậy, việc thiết kế dịch vụ tốt sẽ giảm tối đa ảnh hưởng lan truyền đến các dịch vụ khác, và cần phải có quy tắc phân luồng để trách tình trạng tắc nghẽn ở một dịch vụ nào đó.

### 5. Giới thiệu về TypeScript

TypeScript là một dự án mã nguồn mở được phát triển bởi Microsoft, nó có thể được coi là một phiên bản nâng cao của Javascript bởi việc bổ sung tùy chọn kiểu tĩnh và lớp hướng đối tượng mà điều này không có ở Javascript. TypeScript có thể sử dụng để phát triển các ứng dụng chạy ở Client-side (Angular2) và Server-side (NodeJS). TypeScript sử dụng tất cả các tính năng của của ECMAScript 2015 (viết tắt là ES6) như classes, modules.
Lí do nên sử dụng Typescript:
 - Dễ phát triển dự án lớn: Với việc sử dụng các kỹ thuật mới nhất và lập trình hướng đối tượng nên TypeScript giúp chúng ta phát triển các dự án lớn một cách dễ dàng.
 - Nhiều Framework lựa chọn: Hiện nay các Javascript Framework đã dần khuyến khích nên sử dụng TypeScript để phát triển.
 - Hỗ trợ các tính năng của Javascript phiên bản mới nhất: TypeScript luôn đảm bảo việc sử dụng đầy đủ các kỹ thuật mới nhất của Javascript, ví dụ như version ECMAScript 2015 (ES6).
 - Là mã nguồn mở: TypeScript là một mã nguồn mở nên người dùng hoàn toàn có thể sử dụng mà không mất phí, bên cạnh đó còn được cộng đồng hỗ trợ.
 - TypeScript là Javscript: Bản chất của TypeScript là biên dịch tạo ra các đoạn mã Javascript nên người dùng có thê chạy bất kì môi trường nào miễn ở đó có hỗ trợ biên dịch Javascript. Ngoài ra bạn có thể sử dụng trộn lẫn cú pháp của Javascript vào bên trong TypeScript, điều này giúp các lập trình viên tiếp cận TypeScript dễ dàng hơn.
 
### 6. Sơ đồ mô tả

#### 6.1. Sơ đồ Use case tổng quát

Sơ đồ Use case của nhóm em gồm 2 sơ đồ, vì các chức năng Quản lý danh mục đều bao gồm các chức năng nhỏ như Thêm, Sửa, Xóa nên nhóm chúng em gom lại thành 1 use case là Quản lý danh mục để sơ đồ Use case dễ nhìn hơn, Quản lý danh mục bao gồm:
- Quản lý danh mục kho thiết bị
- Quản lý danh mục tên thiết bị
- Quản lý danh mục loại thiết bị
- Quản lý danh mục đơn vị tính
- Quản lý danh mục nhóm thiết bị
- Quản lý danh mục phân loại chất lượng
- Quản lý danh mục chủng loại thiết bị
- Quản lý danh mục tình trạng hoạt động
- Quản lý danh mục bảo hành
- Quản lý danh mục thiết bị
  
![](https://nhathao2000.000webhostapp.com/UseCase.PNG)

Sơ đồ Use case này gồm 2 nhóm Actor đó là Thủ kho và Trưởng phòng, Thủ kho sẽ là người có các quyền quản lý trang thiết bị, bao gồm cả việc lập phiếu nhập, xuất hay chuyển kho, khi Thủ kho lập một phiếu nhập, xuất kho hay chuyển kho nào đó, phiếu đó sẽ được gửi đến Trưởng phòng để yêu cầu duyệt phiếu, khi phiếu được duyệt, các trang thiết bị sẽ được nhập vào kho.

#### 6.2. Sơ đồ Use case Quản lý danh mục

![](https://nhathao2000.000webhostapp.com/UseCase02.PNG)

#### 6.3. Sơ đồ lớp

![](https://nhathao2000.000webhostapp.com/ClassDiagram.png)

Bảng User chỉ là để tạm vì chúng em chưa biết được bảng User gồm những thuộc tính nào và để lấy mã của admin thì mình sẽ dùng công nghệ nào.

#### 6.4. Sơ đồ tuần tự

##### 6.4.1. Sơ đồ tuần tự Quản lý danh mục

Các chức năng con của các chức năng Quản lý các danh mục đều được thực hiện như nhau nên chúng em gom các sơ đồ tuần tự lại thành 3 sơ đồ chính, đó là Thêm danh mục, Sửa danh mục và Xóa danh mục:

###### 6.4.1.2. Sơ đồ tuần tự Thêm danh mục

![](https://nhathao2000.000webhostapp.com/SDTT_ThemDanhMuc.png)

###### 6.4.1.2. Sơ đồ tuần tự Sửa danh mục

![](https://nhathao2000.000webhostapp.com/SDTT_SuaDanhMuc.png)

###### 6.4.1.3. Sơ đồ tuần tự Xóa danh mục

![](https://nhathao2000.000webhostapp.com/SDTT_XoaDanhMuc.png)

##### 6.4.2. Sơ đồ tuần tự Nhập xuất kho NCC

###### 6.4.2.1. Sơ đồ tuần tự Nhập kho NCC

![](https://nhathao2000.000webhostapp.com/SDTT_NhapKhoNCC.png)

###### 6.4.2.2. Sơ đồ tuần tự Xuất kho NCC

![](https://nhathao2000.000webhostapp.com/SDTT_XuatKhoNCC.png)

###### 6.4.2.3. Sơ đồ tuần tự Sửa thông tin thiết bị

![](https://nhathao2000.000webhostapp.com/SDTT_SuaThongTinThietBi.png)

###### 6.4.2.4. Sơ đồ tuần tự In phiếu

![](https://nhathao2000.000webhostapp.com/SDTT_InPhieu.png)

##### 6.4.3. Sơ đồ tuần tự Chuyển kho

![](https://nhathao2000.000webhostapp.com/SDTT_ChuyenKho.png)

##### 6.4.4. Sơ đồ tuần tự Tra cứu tồn kho

![](https://nhathao2000.000webhostapp.com/SDTT_TraCuuTonKho.png)

##### 6.4.5. Sơ đồ tuần tự Tra cứu thông tin chuyển kho

![](https://nhathao2000.000webhostapp.com/SDTT_TraCuuTTChuyenKho.png)

##### 6.4.6. Sơ đồ tuần tự Sửa chữa thiết bị

![](https://nhathao2000.000webhostapp.com/SDTT_SuaChuaThietBi.png)

##### 6.4.7. Sơ đồ tuần tự Cập nhật trạng thái thiết bị

![](https://nhathao2000.000webhostapp.com/SDTT_CapNhatTrangThaiThietBi.png)

##### 6.4.8. Sơ đồ tuần tự Import danh mục thiết bị

![](https://nhathao2000.000webhostapp.com/SDTT_ImportDanhMucThietBi.png)

### 7. Công cụ Jhipster

JHipster là một nền tảng phát triển để nhanh chóng tạo, phát triển và triển khai các ứng dụng web hiện đại và kiến ​​trúc dịch vụ vi mô. Nền tảng này hỗ trợ nhiều công nghệ giao diện người dùng, bao gồm Angular, React và Vue. Có thể còn hỗ trợ ứng dụng di động cho Ionic và React Native! Về phần phụ trợ, Jhipster hỗ trợ Spring Boot (với Java hoặc Kotlin), Micronaut, Quarkus, Node.js và .NET. 

#### 7.1. Client side

Jhipster hỗ trợ nhiều công nghệ người dùng,  bao gồm Angular, React và Vue.Có thể còn hỗ trợ ứng dụng di động cho Ionic và React Native!
![](https://nhathao2000.000webhostapp.com/39141588-d471-4faf-aaa5-c50fbc9a37ba.png)

#### 7.2. Server side

 Jhipster có thể hỗ trợ Spring Boot (với Java hoặc Kotlin), Node.js và .NET.
![](https://nhathao2000.000webhostapp.com/2e292e0f-0ab8-4eac-987d-fa352d43df20.png)

#### 7.3. Deployment

Jhipster có thể triển khai với Docker và Kubernetes.  Jhipster hỗ trợ triển khai cho AWS, Azure, Cloud Foundry, Google Cloud Platform, Heroku và OpenShift.
 ![](https://nhathao2000.000webhostapp.com/70452aa0-1ec8-41ad-b205-a879bd84e5bb.png)
 
### 8. Angular trong Jhipster

#### 8.1. Cấu trúc dự án

Client code của một dự án Jhipster nằm dưới đường dẫn *src/main/webapp* ở đây chúng ta có thể tạo và thiết kế giao diện ứng dụng
![](https://nhathao2000.000webhostapp.com/Angular/Capture.PNG)

- **i18n**

  Jhipster sử dụng ngx-translate cho mục đích dịch. Ta có thể chỉnh sửa giao diện từng ngôn ngữ bằng cách truy cập vào thư mục *src/main/webapp/i18n*
![](https://nhathao2000.000webhostapp.com/Angular/Capture02.PNG)

- **Thư viện ng-jhipster**

  Thư viện ng-jhipster chứa các chức năng tiện ích và các thành phần phổ biến được sử dụng bởi các ứng dụng Angular 2+. Chúng bao gồm:

  - Chỉ thị xác thực
  - Các thành phần quốc tế hóa
  - Các đường ống thường được sử dụng như viết hoa, sắp xếp thứ tự và cắt bớt từ
  - Base64, dịch vụ xử lý ngày tháng và phân trang
  - Hệ thống thông báo
  
- **Angular CLI**

  - Angular CLI là một công cụ để phát triển, xây dựng và duy trì các ứng dụng Angular. JHipster tạo tệp cấu hình Angular CLI, do đó, quy trình công việc Angular CLI hoạt động với JHipster.

  - Việc tích hợp này được thực hiện bằng cách tạo một tệp angular.json trong thư mục gốc của ứng dụng và thêm các phần phụ thuộc của nó vào tệp package.json.
 
#### 8.2. Ứng dụng của Angular trong JHipster

- Tạo và cho phép tùy chỉnh giao diện người dùng cho 1 entity: Chúng ta sử dụng cả Angular và Bootstrap để tạo giao diện người dùng.
- Bên cạnh đó các hàm được sử dụng trong file Typescript cho phép người sử dụng thêm, sửa hoặc xóa dữ liệu khỏi cơ sở dữ liệu.



 



 






  

