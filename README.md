Вопросы на собеседование iOS-разработчика
==
Тем: много  | Вопросов: дофига

<span style="font-family: 'Raleway';">

</span>

(неподходит, потому что не показывает что человек реально разбтрается в коде) Programming:
--------
- Что такое `куча (heap)` и `стэк (stack)`? В какой памяти создаются объекты, примитивные типы и блоки?
- Что такое `полиморфизм`?
- Что такое `инкапсуляция`? Что такое `нарушение инкапсуляции`?
- Чем `абстрактный класс` отличается от `интерфейса`?
- Что такое сериализация объекта?
- Что такое `регулярные выражения` (regular expression)?
- Что такое `перегрузка операторов (operator overloading)`?
- Что такое `указатель` (pointer)?
- Что такое `функция` (function)?
- Как передавать переменную как ссылку?
- Что такое `класс`?
- Что такое `объект`?
- Что такое `интерфейс`?
- Когда и почему мы используем объект вместо структур?

Swift
----------
- `Фундаментальные` типы и `коллекции`? 
- Aттрибут `@UIApplicationMain` ?
- Что такое `Bridge Header`? Как использовать Objective-C код в Swift проекте?
- Оператор `guard`?
- `Интерполяция` vs `конкатенация` строк?
- `let` vs `var`?
- `typealias`? Создание своего собственного типа?
- nil в Swift vs nil в Objective-C? Различия?
- Оператор `??`?


Objective-C, Foundation:
------------------------
- Что такое `свойство`?
- Директива `@synthesize`, `@dynamic`, чем отличаются друг от друга?
- В чем разница между `точечной нотацией` и использованием квадратных скобок?
- Как правильно реализовать сеттер для свойства с параметром retain?
- Есть ли `приватные и защищенные` методы в Objective-C? 
- Чем `категория` отличается от `категории продолжения класса` (extension, наименованная категория)?
- Можно ли добавить `ivar` в категорию?
- Когда лучше использовать `категорию`, а когда `наследование`?
- `Формальный и неформальный (informal)` протокол? `Протоколы (protocols)`: основные отличия между c#/java интерфейсами и Objective-C протоколами? Что делать в случае если класс не реализует какой-то метод из протокола?
- Что происходит когода мы пытаемся вызвать метод у nil указателя? Разница между nil и Nil и [NSNull null]?
- Что такое `селектор (selector)`? Как его вызвать? как отложить вызов селектора? Что делать если селектор имеет много параметров? `(NSInvocation)`
- Какая разница между использованием селекторов, делегатов и блоков?
- Что такое `KVC`? Когда его нужно использовать?
- Что такое `KVO`? Когда его нужно использовать? Методы для обозревания объектов? Работает ли `KVO с instance переменными (полями)` объекта?
- Какие существуют `root классы` в iOS? Для чего нужны `root классы`? 
- Что такое `тип id`. Что случится во время компиляции если мы посылаем сообщение объекту `типа id`? Что случится во время выполнения если этот метод существует?
- Цепочка ответсвенности, что происходит с методом после того как он не нашелся в объекте класса, которому его вызвали (в сторону forwardInvocation:)?
- Что такое `указатель isa`? Для чего он нужен?
- В чем разница между `NSArray и NSMutableArray`? непотоко-безопасный NSMutableArray?
- Чем отличается `NSSet от NSArray`? Какие `операции` происходят быстро в `NSSet` и какие в `NSArray`?
- Как удалить объект в ходе итерации по циклу?
- Какой контент лучше хранить в `Documents`, а какой в `Cache`?
- Как добавить свойство в существующий объект с закрытой реализацией? Можно ли это сделать через runtime?

iOS Platform:
------------
- Какие бывают `состояния` (states) у приложения?
- Жизненный цикл приложения?
- Каковы самые важные методы делегирования в приложении, с которыми будет сталкиваться разработчик?
- Какого разрешение экранов iphon'ов, и в чем разница между `points (точками)` и `пикселями (pixels)`?
- Что такое `responder chain`?
- Какие типы нотификаций есть в iOS?
- Как работают `push нотификации`?
- Какие ограничение есть у платформы iOS?
- Какие ограничение есть у платформы tvOS?
- Что делает подписание кода (code signing)?
- Что такое ABI?
- Что такое #keyPath()?
- Что IGListKit дает разработчикам?
- Что такое биткод (bitcode)?
- Какие есть ограничения (limits) у SiriKit?
- Что нового в iOS 12?
- Как получить токен устройства (device token)?
- Какие ограничения (limits) у Remote Notifications?

Memory Management:
------------------
- Объявление свойств c атрибутами: `retain`, `assign`, `nonatomic`, `readonly`, `copy`, `weak`, `strong`, `unsafe_unretained`?
- Как происходит `ручное управление памятью - MRC` в iOS?
- `autorelease vs release`?
- Что означает `ARC`?
- `Atomic vs nonatomic`. Чем отличаются? Как вручную переопределить atomic/nonatomic сеттер в не ARC коде?
- Вопрос о `циклах в графах владения` (retain cycle)? 
- Как `использовать` self внутри блоков? Приведите пример `retain cycle` в блоке?
- Что такое `autorelease pool`?
- Что такое `runLoop` `(NSAutoreleasePool)`, когда он используется? `(timers, nsurlconnection ...)`?
- Как происходит обработка `memory warning`(предупреждение о малом  количестве памяти)? Зависит ли обработка от версии iOS, как мы должны их обрабатывать?
- Когда нужно использовать метод `retainCount` (никогда, почему?) :)))
- С подвохом: как работает `сборщик мусора` в iOS? :)))
- Нужно ли `ретейнить` (посылать сообщение retain) `делегаты`?
- Опишите правильный способ управления памятью выделяемой под `Outlet'ы`?

Networking:
----------
- Преимущества и недостатки `синхронного и асинхронного` соединения?
- Что означает `http, tcp`?
- REST, HTTP, JSON. Что это?
- Какие различия между `HEAD, GET, POST, PUT`? 
- Как загрузить что-то из интернета? В чем разница между `синхронными и асинхронными запросами`? Небольшое задание. Опишите как загрузить изображение из интернета и отобразить его в ImageView — все это должно происходить после нажатия кнопки.
- Что такое REST (Restful)?
- Какую JSONSerialization имеет ReadingOptions?

Multithreading:
---------------
- Зачем мы используем synchronized?
- В чем разница между синхронным и асинхронным таском (задачей)?
- Что такое блоки (blocks)?
- Какие типы блоков вы знаете (глобальные/локальные, heap/stack)?
- Что такое обработчик завершения (completion handler)?
- Что такое параллелизм (concurrency)?
- Блокировки читателей-писателей (readers-writers lock)?
- Как многопоточность работает с `UIKit`?
- Как запустить селектор в `(фоновом) потоке`?
- Как запустить `поток (thread)`? Что первым нужно сделать при запуске `потока`?
- Что такое `GCD`? Как `GCD` связан с многопоточностью? Типы queue и queue == thread?
- `NSOperation` vs `GCD`?
- Что такое Dispatch Group?
- NSOperation — NSOperationQueue — NSBlockOperation?
- Что такое `deadlock`?
- Что такое `livelock`?
- Что такое `семафор (semafor)`?
- Что такое `мьютекс (mutex)`?
- `Асинхронность` vs `многопоточность`. Чем отличаются?
- Какие технологии в iOS возможно использовать для работы с потоками. Преимущества и недостатки.
- Чем отличается `dispatch_async от dispatch_sync`?

UIKit:
------
- Разница между свойствами `bounds и frame` объекта UIView? Понимание системы координат?
- Цикл жизни `View Controller`?
- Что такое `View` (представление) и что такое `window` и цикл жизни `UIView`?
- Что такое `Responder Chain` (цепочка обязанностей, `паттерн chain of responsibility`, на примере UI компонентов iOS ), `becomeFirstResponder`.
- Что означают `IBOutlet` и `IBAction`, для чего они нужны, и что значат для препроцессора?
- Как работает `UITableView`? Жизненный цикл UITableView?
- Что можно сделать если клавиатура при появлении скрывает важную часть интерфейса?
- Почему мы должны `релизить IBOutlet'ты` во viewDidUnload?
- Что такое `awakeFromNib`, в чем разница между `xib и nib` файлами?
- Иерархия наследования UIButton.
- В чем разница CollectionViews & TableViews?
- Что такое UIStackView?
- Что такое Autolayout?

CoreAnimation, CoreGraphics:
----------------------------
- Что такое `CALayer`? 
- Чем отличается `UIView от CALayer`?
- Какие типы `CALayer` есть?
- Чем отличается `UIView based Animation от Core Animation`?
- Можно ли `отследить изменение alpha`, через KVO в CALayer?
- Тайминги в `CoreAnimation`?
- Что такое `backing store`?
- Чем отличаются `аффинные преобразования от трехмерных`?
- Нужно ли `ретейнить (посылать сообщение retain)` делегат для `CAAnimation`?


CoreData, Persistency:
----------------------
- Какие есть типы хранилищ (data percistency) и какую стратегию хранения использовать в том или ином случае?
- Какие есть лимиты у JSON/PLIST?
- Что такое Keychain?
- Какие есть лимиты у SQLite?
- Какие есть преимущества у Realm?
- Что такое `нормализация` данных?
- Что такое `Core Data`?
- Что такое NSFetchRequest?
- Что такое NSPersistentContainer?
- Использовали ли `NSFetchedResultsController`? Почему? 
- Что такое `контекст (Managed object context)`? Как происходят `изменения в NSManagedObjectContext`?
- Что такое `Persistent store coordinator`? Зачем нужен `NSPersistentStoreCoordinator`?
- Зачем нужно делать `двустороннии связи` в таблицах?
- Что таке `Fetched Property` и особенности работы с ним по сравнению с обычной связью?
- Что такое `Fault` и зачем он нужен?
- В каких случаях лучше использовать `SQLite`, а в каких `Core Data`?
- Какие есть нюансы при использовании `Core Data в разных потоках`? Как `синхронизировать данные между потоками`(Как синхронизировать контекст)? Синхронизация разных типов NSManagedObjectContext (получение и изменение данных в child контекстах)? 
- Как использовать `СoreData` совместно с `многопоточностью`?
- Что такое `NSManagedObjectId`? Можем ли мы сохранить его на потом если приложение закроется?
- Какие `типы хранилищ` поддерживает CoreData?
- Что такое `ленивая загрузка (lazy loading)`? Что ее связывает с CoreData? Опишите ситуация когда она может быть полезной?


Паттерны:
--------
- Что такое паттерн `Фабрика` (Factory)?
- Что такое паттерн `Фасад` (Facade)?
- Что такое паттерн `Декоратор` (Decorator)?
- Что такое паттерн `Адаптер` (Adapter)?
- Что такое паттерн `Наблюдатель` (Observer)?
- Что такое паттерн `Мементо` (Memento)?
- Назовите основные отличия `синглтона` от `статического класса`, и когда следует использовать один, а когда другой? 
- Как пересоздать синглтон? Можно ли `обнулить объект синглтона`?

Git:
----
- В чем разница между SVN и Git?
- Какая команда Git позволяет объединить коммиты?
- Какая команда Git позволяет нам найти плохие коммиты?
- Какая команда Git сохраняет ваш код без коммита?


Architecture
------------
- SOLID?
- Принципы `DRY`?
- Принципы `KISS`? 
- Что такое `IoC`? 
- Что такое protocol oriented programming?
- What is the difference open & public access level?
- What is the difference fileprivate & private access level?
- Что такое внутренний доступ (internal access)?
- Расскажите о `паттерне MVC`. Чем отличается `пассивная` модель от `активной`?
- Паттерн `MVC vs MVP vs MVVM`? https://habrahabr.ru/post/215605/
- Что такое `VIPER` архитектура?
- Clean Architecture?

Dependency Injection
--------------------
- Где мы используем Dependency Injection?
- Когда подходящее время для внедрения зависимостей (dependency injection) в наши проекты?
- Каковы главные цели фреймворков (framework)?
- Объясните разницу между SDK и Framework?
- Какие библиотеки DI вы знаете?

Unit Testing
------------
- Что такое `TDD` vs.`BDD`?
- Что такое `DDD`?
- Что такое RGR ( Red — Green — Refactor )?
- Объясните “Arrange-Act-Assert”?
- Что такое Code Coverage (покрытие кода)?
- Какие преимущества в написании тестов в приложениях?
- Опишите Test Driven Development в трех простых правилах?
- Что такое TDD?
- Что такое Continuous Integration?
- Чем отличается Mock от Stub. (mock - имитация поведения, stub - вводные данные)


Code Puzzels:
-------------

- Что произойдет здесь (компиляция  + время выполнения): 

```objc
NSString *s = [NSNumber numberWithInt:3]; 
int i = [s intValue];
```

- Что не так с этим кодом? Зачем нужны `инициализаторы`?

```objc
[[[SomeClass alloc] init] init];
```

- Сработает ли `таймер`? Почему? 

```objc
void startTimer(void *threadId) {
   [NSTimer  scheduleTimerWithTimeInterval:10.0f 
      target:aTarget 
          selector:@selector(tick: ) 
          userInfo:nil
           repeats:NO];
}

pthread_create(&thread, NULL, startTimer, (void *)t);
```

- Какой метод вызовется: класса A или класса B? Как надо изменить код, чтобы вызвался метод класса A?

```objc
@interface A : NSObject
- (void)someMethod;
@end

@implementation A
- (void)someMethod {
    NSLog(@"This is class A");
}
@end

@interface B : A
@end

@implementation B
- (void)someMethod  {
    NSLog(@"This is class B");
}
@end

@interface C : NSObject
@end

@implementation C
- (void)method  {
    A *a = [B new];
    [a someMethod];
}
```

- В каких случаях лучше использовать `strong`, а в каких `copy` для NSString? Почему?

```objc
@property (nonatomic, strong) NSString *someString;
@property (nonatomic, copy) NSString *anotherString;
```

- Что выведется в консоль? Почему?

```objc
- (BOOL)objectsCount {
    NSMutableArray *array = [NSMutableArray new];
    for (NSInteger i = 0; i < 1024; i++) {
        [array addObject:[NSNumber numberWithInt:i]];
    }
    return array.count;
}

- (void)someMethod {
    if ([self objectsCount]) {
        NSLog(@"has objects");
    }
    else {
        NSLog(@"no objects");
    }
}
```

- Выведется ли в дебагер «Hello world»? Почему?

```objc
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
    dispatch_sync(dispatch_get_main_queue(), ^{
        NSLog(@"Hello world");
    });

   /* Another implementation */
   return YES;
}
```

- Что выведется в консоль?

```objc
 dispatch_async(dispatch_get_main_queue(), ^
    {
        NSLog(@"A %d", [object retainCount]);
        dispatch_async(dispatch_get_main_queue(), ^{
            NSLog(@"B %d", [object retainCount]);
        });
        NSLog(@"C %d", [object retainCount]);
    });
    NSLog(@"D %d", [object retainCount]);
```

- Что произойдет при исполнении следующего кода? 

```objc
Ball *ball = [[[[Ball alloc] init] autorelease] autorelease];
```
