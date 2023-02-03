About me
### Hi I'm Sergey Serdyuk 👋

I'm Junior Software Engineer. My commercial development experience is just under one year. I have good knowledge in Java development. 
<p align='center'>
   <a href="https://github-readme-stats.vercel.app/api?username=serdyuksb1982&show_icons=true&count_private=true"><img
           height=150
           src="https://github-readme-stats.vercel.app/api?username=serdyuksb1982&show_icons=true&count_private=true"/></a>
   <a href="https://github.com/serdyuksb1982/serdyuksb1982/edit/serdyuksb1982/a/github-readme-stats"><img height=150
                                                                  src="https://github-readme-stats.vercel.app/api/top-langs/?username=serdyuksb1982&layout=compact"/></a>
</p>


<p align='center'>
   📫 My resume on HH: <a href="https://mytischi.hh.ru/resume/3ad4d79dff0976e8260039ed1f4f756e6d6265">serdyuksb</a>     
</p>

<p align='center'>
   📫 How to reach me: <a href='mailto:serdyuksb@gmail.com'>serdyuksb@gmail.com</a>     
</p>

<p align='center'>    
   📫 My tel: 8-926-760-27-01
</p>


## 🛠 Technical Stack
*   Java language
*   MySQL, PostgreSQL, MongoDB, Flyway
*   Spring Framework, Spring Boot, Spring Test, Spring Data Jpa, Spring Jdbc template, Spring Cloud Contract and so on...
*   Maven Apache, Intellij Idea, Atlassian Jira
*   GitHub

## 🛠 Educational literature
*   «Java 8. Руководство для начинающих», Герберт Шилдт;
*   «Алгоритмы на Java», Роберт Сэджвик | Кэвин Уэйн;
*   «Java concurrency in practice», Гетц Брайан;
*   «Тайный код информатики», Чарльз Петцольд;
*   «Грокаем алгоритмы», Бхаргава Адитья.


<div align="center" style="margin: 40px 0">
   <a href="https://github.com/serdyuksb1982&/github-profile-views-counter">
       <img width="175px" src="https://komarev.com/ghpvc/?username=serdyuksb1982&&color=DE002D">
   </a>
</div>

## 🛠 Spring learning -> https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans
1.1. Знакомство с контейнером и Bean Spring IoC:
  * основа для контейнера IoC Spring: org.spingframework.beans and org.springframework.context. Interface BeanFactory, WebApplicationContext for Web.
  *  ![container-magic](https://user-images.githubusercontent.com/92222969/216593994-1559644f-7fb1-4130-aa6b-058c9d69b6d6.png).
  
1.2.1. Метаданные конфигурации:
  * исп. XML; на основе аннотаций; конфигурация на основе Java (@Configuration, @Bean, @Import, и @Depends).
  
1.2.2. Создание экземпляра класса:
  * ApplicationContext context = new ClassPathXmlApplicationContext("services.xml", "daos.xml");
  * возможно составление метаданных конфигурации на основе XML.
  
1.2.3. Использование контейнера:
  * // create and configure beans
ApplicationContext context = new ClassPathXmlApplicationContext("services.xml", "daos.xml");

   // retrieve configured instance
   PetStoreService service = context.getBean("petStore", PetStoreService.class);

   // use configured instance
   List<String> userList = service.getUsernameList().
   
1.3. Обзор компонентов.
  * Контейнер Spring IoC управляет одним или несколькими компонентамию Внутри контейнера определения компонентов представлены в виде BeanDefinition объектов, которые с 
  содержат ряд метаданных.

1.3.2. Создание экземпляров компонентов:
  * с помощью конструктора  
         public class ClientService {
         private static ClientService clientService = new ClientService();
         private ClientService() {}

         public static ClientService createInstance() {
            return clientService;
         }
      }
  * с помощью метода фабрики экземпляров:
         public class DefaultServiceLocator {

         private static ClientService clientService = new ClientServiceImpl();

         public ClientService createClientServiceInstance() {
            return clientService;
         }
      }
   
