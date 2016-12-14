**Формат заголовка актора: артефакт имя\_зависимости имя\_класса**

- [get-session-actor GetSessionActor GetSessionActor](#get-session-actor-getsessionactor-getsessionactor)
- [error-handling-actor ErrorHandlingActor ErrorHandlingActor](#error-handling-actor-errorhandlingactor-errorhandlingactor)
- [actors.user_role_check UserRoleCheck UserRoleCheck](#actors-user_role_check-userrolecheck-userrolecheck)
- [upsert-document-actor UpsertDocumentActor UpsertDocumentActor](#upsert-document-actor-upsertdocumentactor-upsertdocumentactor)
- [delete-from-cached-collection-actor DeleteFromCachedCollectionActor DeleteFromCachedCollectionActor](#delete-from-cached-collection-actor-deletefromcachedcollectionactor-deletefromcachedcollectionactor)
- [delete-document-from-collection-actor DeleteDocumentFromCollectionActor DeleteFromCollectionActor](#delete-document-from-collection-actor-deletedocumentfromcollectionactor-deletedocumentfromcollectionactor)
- [upsert-in-to-collection-actor UpsertInToCollectionActor UpsertInToCollectionActor](#upsert-in-to-collection-actor-upsertintocollectionactor-upsertintocollectionactor)
- [timestamp-generator-actor TimestampGeneratorActor TimestampGeneratorActor](#timestamp-generator-actor-timestampgeneratoractor-timestampgeneratoractor)
- [get-document-by-id-actor GetDocumentByIdActor GetDocumentByIdActor](#get-document-by-id-actor-getdocumentbyidactor-getdocumentbyidactor)
- [copy-field-actor CopyFieldActor CopyFieldActor](#copy-field-actor-copyfieldactor-copyfieldactor)
- [handle-user-info-transactional-actor HandleUserInfoTransactionalActor HandleUserInfoTransactionalActor](#handle-user-info-transactional-actor-handleuserinfotransactionalactor-handleuserinfotransactionalactor)
- [add-user-to-group-handle-user-info-transactional-actor-strategy AddUserToGroupHandleUserInfoTransactionalActorStrategy AddUserToGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)](#add-user-to-group-handle-user-info-transactional-actor-strategy-addusertogrouphandleuserinfotransactionalactorstrategy-addusertogrouphandleuserinfotransactionalactorstrategy-implements-ihandleuserinfotransactionalstrategy)
- [user-info-commons](#user-info-commons)
    - [DBService DBService](#dbservice-dbservice)
    - [SessionsService](#sessionsservice)
- [upsert-field-in-list-document UpsertFieldInListDocumentActor UpsertFieldInListDocumentActor](#upsert-field-in-list-document-upsertfieldinlistdocumentactor-upsertfieldinlistdocumentactor)
- [check-value-absence-in-db-actor CheckValueAbsenceInDbActor CheckValueAbsenceInDbActor](#check-value-absence-in-db-actor-checkvalueabsenceindbactor-checkvalueabsenceindbactor)
- [remove-user-from-group-handle-user-info-transactional-actor-strategy RemoveUserFromGroupHandleUserInfoTransactionalActorStrategy RemoveUserFromGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)](#remove-user-from-group-handle-user-info-transactional-actor-strategy-removeuserfromgrouphandleuserinfotransactionalactorstrategy-removeuserfromgrouphandleuserinfotransactionalactorstrategy-implements-ihandleuserinfotransactionalstrategy)
- [remove-group-handle-user-info-transactional-actor-strategy RemoveGroupHandleUserInfoTransactionalActorStrategy RemoveGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)](#remove-group-handle-user-info-transactional-actor-strategy-removegrouphandleuserinfotransactionalactorstrategy-removegrouphandleuserinfotransactionalactorstrategy-implements-ihandleuserinfotransactionalstrategy)
- [upsert-user-handle-user-info-transactional-actor-strategy UpsertUserHandleUserInfoTransactionalActorStrategy UpsertUserHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)](#upsert-user-handle-user-info-transactional-actor-strategy-upsertuserhandleuserinfotransactionalactorstrategy-upsertuserhandleuserinfotransactionalactorstrategy-implements-ihandleuserinfotransactionalstrategy)
- [upsert-group-handle-user-info-transactional-actor-strategy UpsertGroupHandleUserInfoTransactionalActorStrategy UpsertGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)](#upsert-group-handle-user-info-transactional-actor-strategy-upsertgrouphandleuserinfotransactionalactorstrategy-upsertgrouphandleuserinfotransactionalactorstrategy-implements-ihandleuserinfotransactionalstrategy)
- [remove-user-handle-user-info-transactional-actor-strategy RemoveUserHandleUserInfoTransactionalActorStrategy RemoveUserHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)](#remove-user-handle-user-info-transactional-actor-strategy-removeuserhandleuserinfotransactionalactorstrategy-removeuserhandleuserinfotransactionalactorstrategy-implements-ihandleuserinfotransactionalstrategy)
- [remove-role-from-group-handle-user-info-transactional-actor-strategy RemoveRoleFromGroupHandleUserInfoTransactionalActorStrategy RemoveRoleFromGroupHandleUserInfoTransactionalActorStrategy](#remove-role-from-group-handle-user-info-transactional-actor-strategy-removerolefromgrouphandleuserinfotransactionalactorstrategy-removerolefromgrouphandleuserinfotransactionalactorstrategy)
- [edit-user-password-handle-user-info-transactional-actor-strategy EditUserPasswordHandleUserInfoTransactionalActorStrategy EditUserPasswordHandleUserInfoTransactionalActorStrategy](#edit-user-password-handle-user-info-transactional-actor-strategy-edituserpasswordhandleuserinfotransactionalactorstrategy-edituserpasswordhandleuserinfotransactionalactorstrategy)
- [edit-own-password-handle-user-info-transactional-actor-strategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy](#edit-own-password-handle-user-info-transactional-actor-strategy-editownpasswordhandleuserinfotransactionalactorstrategy-editownpasswordhandleuserinfotransactionalactorstrategy)
- [edit-own-password-handle-user-info-transactional-actor-strategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy](#edit-own-password-handle-user-info-transactional-actor-strategy-editownpasswordhandleuserinfotransactionalactorstrategy-editownpasswordhandleuserinfotransactionalactorstrategy)
- [authenticate-handle-user-info-transactional-actor-strategy AuthenticateHandleUserInfoTransactionalActorStrategy AuthenticateHandleUserInfoTransactionalActorStrategy](#authenticate-handle-user-info-transactional-actor-strategy-authenticatehandleuserinfotransactionalactorstrategy-authenticatehandleuserinfotransactionalactorstrategy)
- [add-user-to-group-handle-user-info-transactional-actor-strategy AddUserToGroupHandleUserInfoTransactionalActorStrategy AddUserToGroupHandleUserInfoTransactionalActorStrategy](#add-user-to-group-handle-user-info-transactional-actor-strategy-addusertogrouphandleuserinfotransactionalactorstrategy-addusertogrouphandleuserinfotransactionalactorstrategy)
- [add-role-to-group-handle-user-info-transactional-actor-strategy AddRoleToGroupHandleUserInfoTransactionalActorStrategy AddRoleToGroupHandleUserInfoTransactionalActorStrategy](#add-role-to-group-handle-user-info-transactional-actor-strategy-addroletogrouphandleuserinfotransactionalactorstrategy-addroletogrouphandleuserinfotransactionalactorstrategy)
- [get-documents-by-filter-over-a-hundred-feature GetDocumentsByFilterOverAHundredFeature GetDocumentsByFilterOverAHundredFeature](#get-documents-by-filter-over-a-hundred-feature-getdocumentsbyfilteroverahundredfeature-getdocumentsbyfilteroverahundredfeature)
- [check-field-not-empty-actor  CheckFieldNotEmptyActor CheckFieldNotEmptyActor](#check-field-not-empty-actor-checkfieldnotemptyactor-checkfieldnotemptyactor)


## get-session-actor GetSessionActor GetSessionActor

По данному идентификатору сессии извлекает из базы данных документ с сессией.
Если сессия не наидена, бросает `ru.vp.studgate.get_session_actor.GetSessionException`.

Интерфейс:
```
public interface GetSessionWrapper {

    // Имя коллекции, в которой будет осуществляться поиск сесиии.
    String getCollectionName() throws ReadValueException;

    // Идентификатор сессии, по которому будет осуществляться поиск.
    String getSessionId() throws ReadValueException;

    // Поле для записи извлечённой из базы сессии.
    void setSession(IObject entries) throws ChangeValueException;
}
```

## error-handling-actor ErrorHandlingActor ErrorHandlingActor

Актор используется для обозначения того, что произошла ошибка.

Актор устанавливает одно из полей в false (поле индикации статуса результата).
Актор копирует сообщение об ошибке из одного поля (поле-источник сообщения) в другое (поле сообщения об ошибке).

Интерфейс:
```
public interface ErrorHandlingWrapper {

    // Поле-источник сообщения об ошибке
    String getErrorMessage() throws ReadValueException;

    // Поле сообщения об ошибке
    void setError(String entries) throws ChangeValueException;

    // Поле индикации статуса результата
    void setSuccess(Boolean entries) throws ChangeValueException;
}
```

## actors.user_role_check UserRoleCheck UserRoleCheck

Проверяет наличие прав у пользователя, от имени которого запущена сессия.
Если права пользователю не даны, бросает `info.smart_tools.smartactors.actors.exception.UserRoleCheckException`.

Интерфейс:
```
public interface UserRoleCheckWrapper {

    // Получает имя коллекции, хранящей список сессий
    String getCollectionName() throws ReadValueException;

    // Получает имя цепочки в карте
    String getMessageMapId() throws ReadValueException;

    // Получает идентификатор сессии
    String getSessionId() throws ReadValueException;

    // Устанавливает флаг:  проверка прав пройдена/не пройдена
    // Сейчас не используется.
    void setResponse(boolean valid) throws ChangeValueException;

    // Отправляет полученный из запроса документ на фронт.
    // Сейчас не используется.
    void setDocument(List<IObject> document) throws ChangeValueException;
}
```

## upsert-document-actor UpsertDocumentActor UpsertDocumentActor

Производит операцию upsert с переданным документом с использованием CachedCollection.

Если попытка upsert документа в коллекцию не удалась, бросает `ru.vp.studgate.update_form_actor.UpsertDocumentActor_CannotUpsert_Exception`

Конструктор:
```
{
    // имя коллекции
    "collectionName": "test",
    // имя ключа, по которому производится кеширование
    "cacheKey": "formKey"
}
```

Интерфейс:
```
public interface UpsertDocumentWrapper {
    // документ для совершения операции
    IObject getDocument() throws ReadValueException;
}
```

## delete-from-cached-collection-actor DeleteFromCachedCollectionActor DeleteFromCachedCollectionActor

Производит операцию delete с переданным документом с использованием CachedCollection: удаляет из CachedCollection и обновляет документ в базе, выствляя isActive=false и обновляя остальные поля.

Если попытка delete документа в коллекции не удалась, бросает `info.smart_tools.smartactors.actors.delete_from_cached_collection.DeleteFromCachedCollectionException`

Конструктор:
```
{
    // имя коллекции
    "collectionName": "test",
    // имя ключа, по которому производится кеширование
    "cacheKey": "formKey"
}
```

Интерфейс:
```
public interface DeleteFromCachedCollectionWrapper {
    // документ для совершения операции
    IObject getDocument() throws ReadValueException;
}
```

## delete-document-from-collection-actor DeleteDocumentFromCollectionActor DeleteDocumentFromCollectionActor

Производит операцию delete с переданным документом из указанной коллекции, в документе обязательным полем является collectionID, по которому производится удаление.

Если попытка delete документа из коллекции не удалась, бросает `ru.vp.admin.delete_document_from_collection_actor.DeleteDocumentFromCollectionActor_CannotDelete_Exception`

Интерфейс:
```
public interface DeleteDocumentFromCollectionWrapper {
    //имя коллекции, из которой необходимо удалить документ
    String getCollectionName() throws ReadValueException;

    // документ для совершения операции
    IObject getDocument() throws ReadValueException;
}
```

## upsert-in-to-collection-actor UpsertInToCollectionActor UpsertInToCollectionActor

Актор имеет два обработчика.

`upsertDocument` обработчик позволяет производить операцию upsert с переднным ему документов.
Интерфейс обработчика имеет специальный метод для записи документа после операции.
Это может быть полезно для получения id документа в случае, если был произведён insert.
Если попытка upsert документа в коллекцию не удалась, бросает `ru.vp.studgate.upsert_in_to_collection_actor.UpsertInToCollectionActor_CannotUpsert_Exception`

`upsertDocuments` обработчик позволяет производить операцию upsert с переднным ему списком документов.
Интерфейс обработчика имеет специальный метод для записи списка документов после операции.
Это может быть полезно для получения id документов в случае, если был произведён insert.
Если попытка upsert какого либо документа в коллекцию не удалась операция для оставшихся документов не производится, обработчик бросает `ru.vp.studgate.upsert_in_to_collection_actor.UpsertInToCollectionActor_CannotUpsert_Exception`


Интерфейс:
```
public interface UpsertDocumentWrapper {

    // Имя коллекции для upsert доумента
    String getCollectionName() throws ReadValueException;

    // Документ
    IObject getDocument() throws ReadValueException;

    // Поле для сохранения документа после операции upsert
    void setDocument(IObject result) throws ChangeValueException;
}
```

`upsertDocuments` обработчик позволяет производить операцию upsert с переднным ему списком документов.
Интерфейс обработчика имеет специальный метод для записи списка документов после операции.
Это может быть полезно для получения id документов в случае, если был произведён insert.
Если попытка upsert документов в коллекцию не удалась, бросает `ru.vp.studgate.upsert_in_to_collection_actor.UpsertInToCollectionActor_CannotUpsert_Exception`

Интерфейс:
```
public interface UpsertDocumentsWrapper {

    // Имя коллекции для upsert доументов
    String getCollectionName() throws ReadValueException;

    // Список документов
    List<IObject> getDocument() throws ReadValueException;

    // Поле для сохранения документов после операции upsert
    void setDocument(List<IObject> result) throws ChangeValueException;
}
```

## timestamp-generator-actor TimestampGeneratorActor TimestampGeneratorActor

Записывает в заданное поле timestamp.
Результирующая строка формируется с использованием `datetime_formatter`.

`handler` обработчик записывает строку, отражающую текущее время в указанное поле документа.

Интерфейс:
```
public interface TimestampGeneratorActorWrapper {
    // Поле для записи timestamp
    void setTimestamp(String timestamp) throws ChangeValueException;
}
```

## get-document-by-id-actor GetDocumentByIdActor GetDocumentByIdActor

`handler` обработчик извлекает из заданной коллекции документ с заданным id.
В случае если ни одного документа не наидено, бросает `ru.vp.studgate.get_document_by_id_actor.GetDocumentByIdActor_CannotFindDocumentById_Exception`.
В случае если наидены несколько документов, возвращает первый из наиденных.

Интерфейс:
```
public interface GetDocumentByIdActorWrapper {

    // Имя коллекции для поиска документа
    String getCollectionName() throws ReadValueException;

    // Идентификатор документа
    String getEntityId() throws ReadValueException;

    // Имя поля для хранения идентификатора документа в базе данных
    String getIdFieldNameInDatabase() throws ReadValueException;

    // Поле для сохранения наиденного документа
    void setDocument(IObject entries) throws ChangeValueException;
}
```


## copy-field-actor CopyFieldActor CopyFieldActor

`handler` обработчик копирует содержимое одного поля в другое поле.

Интерфейс:
```
public interface CopyFieldActorWrapper {

    // Откуда копировать
    Object getFrom() throws ReadValueException;

    // Куда копировать
    void setTo(Object o) throws ChangeValueException;
}
```

## handle-user-info-transactional-actor HandleUserInfoTransactionalActor HandleUserInfoTransactionalActor

Актор может использоваться как синхронизатор обращений чтения-записи информации о ролях групп, группах пользователей,
информации о сессиях.

Расширяемость набора действий с информацией о ролях, пользователях, сессиях и группах реализована через стратегии.

`handler` обработчик по названию стратегии разрешает её как зависимость типа `IHandleUserInfoTransactionalStrategy`
и вызывает её метод `handle(HandleTransactionalActorWrapper m)`, передавая своё сообщение в качестве параметра метода.

Интерфейс:
```
public interface HandleTransactionalActorWrapper {
    // Имя зависимости стратегии
    String getStrategyName() throws ReadValueException;
    // Строка, позволяющая передать стратегии параметры инициализации
    String getStrategyParams() throws ReadValueException;
    // Метод позволяет стратегии извлеч параметры запроса из сообщения
    IObject getMessage() throws ReadValueException;
}
```

## add-user-to-group-handle-user-info-transactional-actor-strategy AddUserToGroupHandleUserInfoTransactionalActorStrategy AddUserToGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)

Стратегия актора `handle-user-info-transactional-actor` (`HandleUserInfoTransactionalActor`), добавляющая пользователя в группу.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"groupIdFieldName\": \"user_groupsID\", \"usersCollectionName\": \"users\", \"groupsCollectionName\": \"user_groups\", \"userGroupsFieldName\": \"groups\", \"userRolesFieldName\": \"roles\", \"groupRolesFieldName\": \"roles\", \"groupUsersFieldName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "cbefa401-a73b-4174-97e2-01f4a8ff48a5",
	"groupId": "fbb651f6-0a7c-4989-85b3-8d7cf0a61d63"
}
```
`groupId` - идентификатор группы, в которую будет добавлен пользователь.

`userId` - идентификатор пользователя, добавляемого в группу.


## user-info-commons

### DBService DBService

Утилитный класс для работы с базой данных.

### SessionsService

Утилитный класс для работы с сессиями пользователей.


## upsert-field-in-list-document UpsertFieldInListDocumentActor UpsertFieldInListDocumentActor

Обновляет через CachedCollection поле в списке документов, удовлетворяющих условию, и, при необходимости, заносит запись в историю.
Если при создании экземпляра класса произошла ошибка, бросает `ru.vp.studgate.upsert_field_in_list_document.UpsertFieldInListDocumentActorException`. Если ошибка произошла во время выполения - `ru.vp.studgate.upsert_field_in_list_document.UpsertFieldInListDocumentException`.

Интерфейс:
```
public interface UpsertFieldInListDocumentWrapper {
    // Получает имя поля, которое необходимо изменить
    String getFieldName() throws ReadValueException;

    // Получает значение поля, которое необходимо установить
    String getFieldValue() throws ReadValueException;

    // Получает имя поля, по которому ищутся записи (совпадение значений)
    String getСonditionName() throws ReadValueException;

    // Получает значение поля для проверки условия
    String getСonditionValue() throws ReadValueException;

    // Получает имя сотрудника, изменившего запись
    String getFirstName() throws ReadValueException;

    // Получает отчество сотрудника, изменившего запись
    String getMiddleName() throws ReadValueException;

    // Получает фамилию сотрудника, изменившего запись
    String getLastName() throws ReadValueException;

    // Получает ID сотрудника, изменившего запись
    String getEntityId() throws ReadValueException;

    // Получает имя коллекции, в которую необходимо занести запись об истории изменений. Если поле пустое, запись истории не производится.
    String getCollectionHistoryName() throws ReadValueException;
}
```

## check-value-absence-in-db-actor CheckValueAbsenceInDbActor CheckValueAbsenceInDbActor

`handler` обработчик проверяет, существует ли в заданной коллекции заданное значение в заданном поле.
В случае если заданное значение в заданном поле уже есть, бросает `ru.vp.studgate.get_document_by_id_actor.CheckValueAbsenceInDbActor_ValueIsPresent_Exception`.
В противном случае не производит никаких действий.

Интерфейс:
```
public interface CheckValueAbsenceInDbActorWrapper {
    // Имя коллекции
    String getCollectionName() throws ReadValueException;

    // Значение для проверки на наличие в коллекции
    String getSupposedAbsenceValue() throws ReadValueException;

    // Имя поля по которому производить поиск значения
    String getDBFieldName() throws ReadValueException;
}
```


## remove-user-from-group-handle-user-info-transactional-actor-strategy RemoveUserFromGroupHandleUserInfoTransactionalActorStrategy RemoveUserFromGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), удаляющая пользователя из
группы.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"groupIdFieldName\": \"user_groupsID\", \"usersCollectionName\": \"users\", \"groupsCollectionName\": \"user_groups\", \"userGroupsFieldName\": \"groups\", \"userRolesFieldName\": \"roles\", \"groupRolesFieldName\": \"roles\", \"groupUsersFieldName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\",\"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "cbefa401-a73b-4174-97e2-01f4a8ff48a5",
	"groupId": "fbb651f6-0a7c-4989-85b3-8d7cf0a61d63"
}
```
`groupId` - идентификатор группы, из которой будет удалён пользователь.

`userId` - идентификатор пользователя, удаляемого из группы.


## remove-group-handle-user-info-transactional-actor-strategy RemoveGroupHandleUserInfoTransactionalActorStrategy RemoveGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), удаляющая группу.

Бросает
`ru.vp.studgate.remove_group_handle_user_info_transactional_actor_strategy.RemoveGroupHandleUserInfoTransactionalActorStrategy_GroupIsNotEmpty_Exception`
в случае, если группа не пуста (в группе есть пользователи).

Параметры стратегии (`getStrategyParams`):

`{\"groupIdFieldName\": \"user_groupsID\", \"groupsCollectionName\": \"user_groups\", \"groupUsersFieldName\": \"users\"}`

Содержание запроса (`getMessage()`):

```
{
	"groupId": "fbb651f6-0a7c-4989-85b3-8d7cf0a61d63"
}
```
`groupId` - идентификатор группы для удаления.


## upsert-user-handle-user-info-transactional-actor-strategy UpsertUserHandleUserInfoTransactionalActorStrategy UpsertUserHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), обновляющая запись о
пользователе в базе данных.

Бросает
`ru.vp.studgate.upsert_user_handle_user_info_transactional_actor_strategy.UpsertUserHandleUserInfoTransactionalActorStrategy_UserNotDefined_Exception`
в случае, если не передан документ-пользователь для записи в
базу данных.

Параметры стратегии (`getStrategyParams`):

`{\"usersCollectionName\": \"users\"}`

Содержание запроса (`getMessage()`):

```
{
	"document": {
	    ... some user contents ...
	}
}
```
`document` - содержимое документа-пользователя.

## upsert-group-handle-user-info-transactional-actor-strategy UpsertGroupHandleUserInfoTransactionalActorStrategy UpsertGroupHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), обновляющая запись о группе
в базе данных.

Бросает
`ru.vp.studgate.upsert_group_handle_user_info_transactional_actor_strategy.UpsertGroupHandleUserInfoTransactionalActorStrategy_GroupNotDefined_Exception`
в случае, если не передан документ-группа для записи в базу данных.

Параметры стратегии (`getStrategyParams`):

`{\"groupsCollectionName\": \"user_groups\"}`

Содержание запроса (`getMessage()`):

```
{
	"document": {
	    ... some group contents ...
	}
}
```
`document` - содержимое документа-группы.


## remove-user-handle-user-info-transactional-actor-strategy RemoveUserHandleUserInfoTransactionalActorStrategy RemoveUserHandleUserInfoTransactionalActorStrategy (implements IHandleUserInfoTransactionalStrategy)
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), удаляющая пользователя.
Процедура удаления пользователя заключается в двух действиях:
1. Исключении пользователя из группы, дающей пользователям право входить на сайт. Идентификатор группы передаётся в стратеги как параметр.
1. Деактивации всех активных сессий пользователя.

Бросает
`ru.vp.studgate.remove_user_handle_user_info_transactional_actor_strategy.RemoveUserHandleUserInfoTransactionalActorStrategy_UserAlreadyRemoved_Exception`
в случае, если пользователь не состоит в группе, дающей право
входа на сайт.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"groupIdFieldName\": \"user_groupsID\", \"usersCollectionName\": \"users\", \"groupsCollectionName\": \"user_groups\", \"userGroupsFieldName\": \"groups\", \"userRolesFieldName\": \"roles\", \"groupRolesFieldName\": \"roles\", \"groupUsersFieldName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\", \"loginGroupId\": \"0a737aae-9cec-4e4d-aaea-1d11eae83390\",\"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "b3abb12b-09d7-440f-bca8-f63510a38b92"
}
```

`userId` - идентификатор пользователя для удаления.

## remove-role-from-group-handle-user-info-transactional-actor-strategy RemoveRoleFromGroupHandleUserInfoTransactionalActorStrategy RemoveRoleFromGroupHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), удаляющая роль из группы.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"groupIdFieldName\": \"user_groupsID\", \"usersCollectionName\": \"users\", \"groupsCollectionName\": \"user_groups\", \"userGroupsFieldName\": \"groups\", \"userRolesFieldName\": \"roles\", \"groupRolesFieldName\": \"roles\", \"groupUsersFieldName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\",\"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"groupId": "eddd9277-5225-4ebc-9890-e59a05ed1363",
	"role": "admin_SomeRoleName"
}
```

`groupId` - идентификатор группы.

`role` - роль для удаления .


## edit-user-password-handle-user-info-transactional-actor-strategy EditUserPasswordHandleUserInfoTransactionalActorStrategy EditUserPasswordHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), изменяющая пароль пользователя.
Может использоваться администратором для смены пароля пользователям.

Бросает
`ru.vp.studgate.edit_user_password_handle_user_info_transactional_actor_strategy.EditUserPasswordHandleUserInfoTransactionalActorStrategy_UserDoesNotExist_Exception`
в случае, если пользователь с переданным id не существует.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"usersCollectionName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\", \"userDBPasswordFieldName\": \"password\", \"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "eddd9277-5225-4ebc-9890-e59a05ed1363",
	"newPassword": "whimRovcang3"
}
```

`userId` - идентификатор пользователя.

`newPassword` - новый пароль.


## edit-own-password-handle-user-info-transactional-actor-strategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), изменяющая пароль пользователя с проверкой старого пароля.
Может использоваться пользователем для смены пароля самому себе.

Бросает
`ru.vp.studgate.edit_own_password_handle_user_info_transactional_actor_strategy.EditOwnPasswordHandleUserInfoTransactionalActorStrategy_UserDoesNotExist_Exception`
в случае, если пользователь с переданным id не существует.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"usersCollectionName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\", \"userDBPasswordFieldName\": \"password\",\"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "eddd9277-5225-4ebc-9890-e59a05ed1363",
	"oldPassword": "whimRovcang3",
	"newPassword": "lavEcWognav4"
}
```

`userId` - идентификатор пользователя.

`oldPassword` - старый пароль пользователя.

`newPassword` - новый пароль пользователя.


## edit-own-password-handle-user-info-transactional-actor-strategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy EditOwnPasswordHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), изменяющая пароль пользователя с проверкой старого пароля.
Может использоваться пользователем для смены пароля самому себе.

Бросает
`ru.vp.studgate.edit_own_password_handle_user_info_transactional_actor_strategy.EditOwnPasswordHandleUserInfoTransactionalActorStrategy_UserDoesNotExist_Exception`
в случае, если пользователь с переданным id не существует.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"usersCollectionName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\", \"userDBPasswordFieldName\": \"password\",\"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "eddd9277-5225-4ebc-9890-e59a05ed1363",
	"oldPassword": "whimRovcang3",
	"newPassword": "lavEcWognav4"
}
```

`userId` - идентификатор пользователя.

`oldPassword` - старый пароль пользователя.

`newPassword` - новый пароль пользователя.

## authorize-handle-user-info-transactional-actor-strategy AuthorizeHandleUserInfoTransactionalActorStrategy AuthorizeHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), выполняющая следующие действия:
1. Авторизация пользователя по id сессии
1. Авторизация пользователя по времени жизни сессии.
1. Авторизация пользователя по ролям/имени цепочки.
1. В случае если пользователь авторизован - продление сессии на заданное количество времени с момента последней авторизации.

Бросает
`ru.vp.studgate.add_role_to_group_handle_user_info_transactional_actor_strategy.AuthorizeHandleUserInfoTransactionalActorStrategy_NotAuthorized_Exception`
в случае, если активная сессия не наидена или если пользователь не авторизован для выполнения действия.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\",\"sessionIdFieldName\": \"sessionId\",\"sessionUserFieldName\": \"user\",\"messageMapIdFieldName\": \"messageMapId\",\"sessionsCollectionName\": \"session\",\"dbSessionIdFieldName\": \"sessionID\",\"sessionTimeToLiveFieldName\": \"sessionTTL\",\"sessionDurationInSeconds\": \"1800\",\"userRolesFieldName\": \"roles\"}`

Содержание запроса (`getMessage()`):

```
{
	"<sessionIdFieldName>": "eddd9277-5225-4ebc-9890-e59a05ed1363",
	"messageMapId": "admin_SomeChain"
}
```

`\<sessionIdFieldName\>` - имя поля устанавливается в параметрах стратегии. Содержит идентификатор сессии пользователя.

`messageMapId` - имя цепочки, для которой проводится авторизация.

## authenticate-handle-user-info-transactional-actor-strategy AuthenticateHandleUserInfoTransactionalActorStrategy AuthenticateHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), выполняющая аутентификацию по
паре логин/пароль и генерирующая сессию в случае успешной
аутентификации.

Идентификатор сгенерированной сессии возвращается в поле, конфигурируемым полем `sessionIdFieldName`

Бросает
`ru.vp.studgate.authenticate_handle_user_info_transactional_actor_strategy.AuthenticateHandleUserInfoTransactionalActorStrategy_AuthenticationError_Exception`
в случае, если пара логин/пароль неверна.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\",\"groupIdFieldName\": \"user_groupsID\",\"usersCollectionName\": \"users\",\"groupsCollectionName\": \"user_groups\",\"userGroupsFieldName\": \"groups\",\"userRolesFieldName\": \"roles\",\"groupRolesFieldName\": \"roles\",\"groupUsersFieldName\": \"users\",\"sessionsCollectionName\": \"session\",\"dbSessionUserIdFieldName\": \"usersID\",\"sessionUserFieldName\": \"user\",\"sessionIdFieldName\": \"sessionID\",\"userLoginFieldName\": \"login\",\"sessionTimeToLiveFieldName\": \"sessionTTL\",\"sessionDurationInSeconds\": \"1800\", \"sessionsAmountPerRequest\": \"100\"}`

Содержание запроса (`getMessage()`):

```
{
	"login": "Upp7Onyurm6",
	"password": "oribrecBom4"
}
```

`login` - логин пользователя.

`password` - цепочка пользователя.

## update-group-handle-user-info-transactional-actor-strategy UpdateGroupHandleUserInfoTransactionalActorStrategy UpdateGroupHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), обновляющая имя группы.

Бросает `ru.vp.admin.update_group_handle_user_info_transactional_actor_strategy.UpdateGroupHandleUserInfoTransactionalActorStrategy_BadRequest_Exception` в случае, если не указано содержимое новой группы или указанная для редактирования группа не наидена.
Бросает `ru.vp.admin.update_group_handle_user_info_transactional_actor_strategy.UpdateGroupHandleUserInfoTransactionalActorStrategy_BadRequest_Exception` в случае, если не указано имя или ID редактируемой группы.

Параметры стратегии (`getStrategyParams`):

`{\"groupsCollectionName\": \"user_groups\",\"groupIdFieldName\": \"user_groupsID\",\"groupNameFieldName\": \"groupName\",\"groupRolesFieldName\": \"roles\",\"groupUsersFieldName\": \"users\"}`

Содержание запроса (`getMessage()`):

```
{
    "document": {
        "<groupNameFieldName>": "some-group-name",
        "<groupIdFieldName>": "admin_SomeChain"
    }
}
```

`\<groupNameFieldName\>` - новое имя группы.

`\<groupIdFieldName\>` - идентификатор переименовываемой группы.


## add-user-to-group-handle-user-info-transactional-actor-strategy AddUserToGroupHandleUserInfoTransactionalActorStrategy AddUserToGroupHandleUserInfoTransactionalActorStrategy
Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), добавляющая пользователя в группу.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"groupIdFieldName\": \"user_groupsID\", \"usersCollectionName\": \"users\", \"groupsCollectionName\": \"user_groups\", \"userGroupsFieldName\": \"groups\", \"userRolesFieldName\": \"roles\", \"groupRolesFieldName\": \"roles\", \"groupUsersFieldName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\",\"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "eb61269f-2302-4c48-9d34-6934af173d18",
	"groupId": "b2e3617c-ec9b-4831-9d96-9d3e3ba214bf"
}
```

`userId` - идентификатор пользователя.

`groupId` - идентификатор группы.


## create-user-handle-user-info-transactional-actor-strategy CreateUserHandleUserInfoTransactionalActorStrategy CreateUserHandleUserInfoTransactionalActorStrategy

Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), создающая нового пользователя на сервере.

Бросает `ru.vp.admin.create_user_handle_user_info_transactional_actor_strategy.CreateUserHandleUserInfoTransactionalActorStrategy_BadRequest_Exception` если в запросе не указан логин или пароль нового пользователя.
Бросает `ru.vp.admin.create_user_handle_user_info_transactional_actor_strategy.CreateUserHandleUserInfoTransactionalActorStrategy_UserAlreadyExists_Exception` если пользователь с таким логином уже существует.

Параметры стратегии (`getStrategyParams`):

`{\"usersCollectionName\": \"users\",\"userLoginFieldName\": \"login\",\"userIdFieldName\": \"usersID\",\"userRolesFieldName\": \"roles\",\"userGroupsFieldName\": \"groups\",\"userPasswordFieldName\": \"password\"}`

Содержание запроса (`getMessage()`):

```
{
    "document": {
    	"\<userLoginFieldName\>": "eb61269f-2302-4c48-9d34-6934af173d18",
    	"\<userPasswordFieldName\>": "b2e3617c-ec9b-4831-9d96-9d3e3ba214bf"
    }
}
```

`userLoginFieldName` - логин пользователя.

`userPasswordFieldName` - пароль пользователя.


## update-user-handle-user-info-transactional-actor-strategy UpdateUserHandleUserInfoTransactionalActorStrategy UpdateUserHandleUserInfoTransactionalActorStrategy

Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), обновляет данные пользователя.

Бросает `ru.vp.admin.update_user_handle_user_info_transactional_actor_strategy.UpdateUserHandleUserInfoTransactionalActorStrategy_BadRequest_Exception` если в запросе не указано поле `document`, не указан логин или id пользователя.
Бросает `ru.vp.admin.update_user_handle_user_info_transactional_actor_strategy.UpdateUserHandleUserInfoTransactionalActorStrategy_LoginAlreadyExists_Exception` если пользователь с указанным логином уже существует.
Бросает `ru.vp.admin.update_user_handle_user_info_transactional_actor_strategy.UpdateUserHandleUserInfoTransactionalActorStrategy_UserForUpdatingNotExists_Exception` если пользователь с указанным ID не наиден.

Параметры стратегии (`getStrategyParams`):

`{\"usersCollectionName\": \"users\",\"userLoginFieldName\": \"login\",\"userIdFieldName\": \"usersID\",\"userRolesFieldName\": \"roles\",\"userGroupsFieldName\": \"groups\",\"userPasswordFieldName\": \"password\"}`

Содержание запроса (`getMessage()`):

```
{
    "document": {
    	"\<userLoginFieldName\>": "someNewLogin",
    	"\<userIdFieldName\>": "b2e3617c-ec9b-4831-9d96-9d3e3ba214bf"
    }
}
```

`userLoginFieldName` - логин пользователя.

`userIdFieldName` - пароль пользователя.


## add-role-to-group-handle-user-info-transactional-actor-strategy AddRoleToGroupHandleUserInfoTransactionalActorStrategy AddRoleToGroupHandleUserInfoTransactionalActorStrategy

Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), добавляющая пользователя в группу.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\", \"groupIdFieldName\": \"user_groupsID\", \"usersCollectionName\": \"users\", \"groupsCollectionName\": \"user_groups\", \"userGroupsFieldName\": \"groups\", \"userRolesFieldName\": \"roles\", \"groupRolesFieldName\": \"roles\", \"groupUsersFieldName\": \"users\", \"sessionsCollectionName\": \"session\", \"dbSessionUserIdFieldName\": \"usersID\", \"sessionUserFieldName\": \"user\", \"sessionsAmountPerRequest\": \"100\", \"sessionTimeToLiveFieldName\": \"sessionTTL\",\"sessionDurationInSeconds\": \"1800\"}`

Содержание запроса (`getMessage()`):

```
{
	"userId": "eb61269f-2302-4c48-9d34-6934af173d18",
	"groupId": "b2e3617c-ec9b-4831-9d96-9d3e3ba214bf"
}
```

`userId` - идентификатор пользователя.

`groupId` - идентификатор группы.


## create-group-handle-user-info-transactional-actor-strategy CreateGroupHandleUserInfoTransactionalActorStrategy CreateGroupHandleUserInfoTransactionalActorStrategy

Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), создающая группу.

Бросает `ru.vp.admin.create_group_handle_user_info_transactional_actor_strategy.CreateGroupHandleUserInfoTransactionalActorStrategy_BadRequest_Exception` в случае некорректного формата запроса (не задано имя группы).
Бросает `ru.vp.admin.create_group_handle_user_info_transactional_actor_strategy.CreateGroupHandleUserInfoTransactionalActorStrategy_NameExist_Exception` в случае, если группа с таким именем уже существует.

Параметры стратегии (`getStrategyParams`):

`{\"groupsCollectionName\": \"user_groups\",\"groupIdFieldName\": \"user_groupsID\",\"groupNameFieldName\": \"groupName\",\"groupRolesFieldName\": \"roles\",\"groupUsersFieldName\": \"users\"}`

Содержание запроса (`getMessage()`):

```
{
    "document": {
        "groupName": "Some goup name!"
        ...
        see user group database entity format
        ...
    }
}
```

`document` - документ группы.


## purge-session-handle-user-info-transactional-actor-strategy PurgeSessionHandleUserInfoTransactionalActorStrategy PurgeSessionHandleUserInfoTransactionalActorStrategy

Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), удаляющая сессию по её id.

Бросает `ru.vp.admin.purge_session_handle_user_info_transactional_actor_strategy.PurgeSessionHandleUserInfoTransactionalActorStrategy_BadRequest_Exception` в случае, если идентификатор сессии не задан.

Параметры стратегии (`getStrategyParams`):

`{\"groupsCollectionName\": \"user_groups\",\"groupIdFieldName\": \"user_groupsID\",\"groupNameFieldName\": \"groupName\",\"groupRolesFieldName\": \"roles\",\"groupUsersFieldName\": \"users\"}`

Содержание запроса (`getMessage()`):

```
{
    "sessionId": "6fa443d4-cabe-49d6-9cc8-0162ce0e5dd0"
}
```

`document` - документ с идентификатором сессии.


## authorize-without-roles-check-handle-user-info-session-actor-strategy AuthorizeWithoutRolesCheckHandleUserInfoActorStrategy AuthorizeWithoutRolesCheckHandleUserInfoActorStrategy

Стратегия актора `handle-user-info-transactional-actor`
(`HandleUserInfoTransactionalActor`), выполняющая следующие действия:
1. Авторизация пользователя по id сессии
1. Авторизация пользователя по времени жизни сессии.
1. Авторизация пользователя по ролям/имени цепочки.
1. В случае если пользователь авторизован - продление сессии на заданное количество времени с момента последней авторизации.

Бросает `ru.vp.admin.authorize_without_roles_check_handle_user_info_session_actor_strategy.AuthorizeWithoutRolesCheckHandleUserInfoActorStrategy_NotAuthorized_Exception` в случае, если идентификатор сессии не задан.
Бросает `ru.vp.admin.authorize_without_roles_check_handle_user_info_session_actor_strategy.AuthorizeWithoutRolesCheckHandleUserInfoActorStrategy_NotAuthorized_Exception` в случае, если активная сессия с указанным ID не наидена.

Параметры стратегии (`getStrategyParams`):

`{\"userIdFieldName\": \"usersID\",\"sessionIdFieldName\": \"sessionId\",\"sessionUserFieldName\": \"user\",\"messageMapIdFieldName\": \"messageMapId\",\"sessionsCollectionName\": \"session\",\"dbSessionIdFieldName\": \"sessionID\",\"sessionTimeToLiveFieldName\": \"sessionTTL\",\"sessionDurationInSeconds\": \"1800\",\"userRolesFieldName\": \"roles\"}`

Содержание запроса (`getMessage()`):

```
{
	"<sessionIdFieldName>": "eddd9277-5225-4ebc-9890-e59a05ed1363",
}
```
`\<sessionIdFieldName\>` - имя поля устанавливается в параметрах стратегии. Содержит идентификатор сессии пользователя.


## get-documents-by-filter-over-a-hundred-feature GetDocumentsByFilterOverAHundredFeature GetDocumentsByFilterOverAHundredActor

`handler` обработчик извлекает все документы заданной коллекции(`даже если их больше 100`), допустимо использование фильтра.
`Warning: не стабильная работа с большим количеством документов.`

Интерфейс:
```
public interface GetDocumentsByFilterOverAHundredActorWrapper {

    // Имя коллекции, в которой будет осуществляться поиск отфильтрованных значений(если фильтр задан).
    String getCollectionName() throws ReadValueException;

    // Строка, по которой будет осуществляться фильтрация.
    String getFilter() throws ReadValueException;

    // метод записывающий результат возвращенный из коллекции, необходим для записи извлеченного массива из базы.
    void setDocument(List<IObject> document) throws ChangeValueException;
}
```


## check-gateway-status-in-gateway-types-actor  CheckGatewayStatusInGatewayTypesActor CheckGatewayStatusInGatewayTypesActor
`handler` проверяет, включен ли шлюз, если хотите применить его к методу оплаты.

Если пытаетесь использовать выключенный шлюз, то бросает исключение `ru.vp.admin.check_gateway_status_in_gateway_types_actor.CheckGatewayStatusInGatewayTypesActorException`.

Интерфейс:
```
public interface CheckGatewayStatusInGatewayTypesActorWrapper {

    // Возвращает матрицу методов оплаты.
    IObject getPaymentMatrix() throws ReadValueException;

    // Возвращает список методов оплаты
    List<IObject> getGateways() throws ReadValueException;
}
```


## check-field-not-empty-actor  CheckFieldNotEmptyActor CheckFieldNotEmptyActor
`handler` проверяет,  поле != null и поле != "".

Если поле пустое или не определено, то выбрасывается исключение `ru.vp.admin.check_field_not_empty_actor.CheckFieldNotEmptyActorException`.

Интерфейс:
```
public interface CheckFieldNotEmptyActorWrapper {

    // Получает значение поля.
    String getFieldValue() throws ReadValueException;
}
```

## check-if-using-document-actor CheckIfUsingDocumentActor CheckIfUsingDocumentActor

По заданным имени коллекции, имени поля-массива и значения-строки, извлекает из базы список документов, содержащих в поле-масиве значение-строку.

Если список наиденных документов не пуст или поиск осуществить не удалось, бросает `ru.vp.admin.check_if_using_document_actor.CheckIfUsingDocumentActorException`.

Интерфейс:
```
public interface CheckIfUsingDocumentActorWrapper {

    // Имя коллекции, в которой будет осуществляться поиск документов.
    String getCollectionName() throws ReadValueException;

    // Название поля-массива, в котором осуществляется поиск значения для поиска
    String getValueField() throws ReadValueException;

    // Искомое в поле-массиве значение
    String getFieldName() throws ReadValueException;

}
```

## uniqueness-check-document-actor UniquenessCheckDocumentActor UniquenessCheckDocumentActor

По заданным имени коллекции, имени поля, значению-строке и значению ID документа проверяет, имеются ли в коллекции документы, имеющие равное указанному значению-строке значение в заданном поле, но отличный от указанного ID идентификатор (имя поля идентификатора считается равным имени коллекции, конкатенированному с суффиксом "ID").

Если список наиденных документов не пуст или поиск осуществить не удалось, бросает `ru.vp.admin.uniqueness_check_document_actor.UniquenessCheckDocumentActorException`.

Интерфейс:
```
public interface UniquenessCheckDocumentActorWrapper {

    // Имя коллекции, в которой будет осуществляться поиск документов.
    String getCollectionName() throws ReadValueException;

    // Искомое значение-строка
    String getValueField() throws ReadValueException;

    // Имя поля, по которому проиводится поиск значения-строки
    String getFieldName() throws ReadValueException;

    // ID документа
    String getID() throws ReadValueException;
}
```


## get-session-info-by-sessionId-actor GetSessionInfoBySessionIdActor GetSessionInfoBySessionIdActor

По заданным имени коллекции и идентификатору сессии извлекает из сессии с заданным ID фамилию с инифиалами, идентификатор пользователя и список его прав.

Если фамилия пользователя неизвестна, она не добавляется в результат.
Если имя пользователя неизвестно, инициал имени не добавляется к результату.
Если отчество пользователя неизвестно, инициал отчества не добавляется к результату.

Если не наидено единственной активной сессии с заданным идентификатором, бросает `ru.vp.admin.get_session_info_by_sessionId_actor.GetSessionInfoBySessionIdException`.

Особенности реализации:
Пустая фамилия при заданных имени и/или отчестве приводит к тому, что результат содержит лидирующий пробел.
Первые буквы фамилии и инициалов вставляются как есть (т.е. без принудительного переключения в верхний регистр).

Интерфейс:
```
public interface GetSessionInfoBySessionIdActorWrapper {

    // Поле для записи фамилии и инициалов
    void setFullName(String s) throws ChangeValueException;

    // Поле для записи идентификатора пользователя
    void setUsersID(String s) throws  ChangeValueException;

    // Поле для записи прав пользователя
    void setPermission(List<String> s) throws ChangeValueException;

    // Идентификатор сессии пользователя
    String getSessionId() throws ReadValueException;

    // Имя коллекции в которой хранятся сессии
    String getCollectionName() throws ReadValueException;
}
```
## transform-actor TransformActor TransformActor

Достаёт из объекта "пользователь" поля: login, password, roles, и ложит их в одноимённые поля. 

Если поле пустое или не определено, то выбрасывается исключение `ru.vp.admin.check_field_not_empty_actor.CheckFieldNotEmptyActorException`.

Интерфейс:
```
public interface TransformActorWrapper {
    //Поле с пользователем
    List<IObject> getUser() throws ReadValueException;
    //Устанавливает поле логин
    void setLogin(String login) throws ChangeValueException;
    //Установка поля пароль
    void setPasswordHashFromDB(String hash) throws ChangeValueException;
    //Установка поля роли
    void setRole(Object role) throws ChangeValueException;
}
```
## print-message-actor PrintMessageActor PrintMessageActor

Выводит с помощью ситемного вывода, объект в виде json строки.

Если поле не может быть сериализованно, то выбрасываеться исключение `ru.vp.admin.timestamp_generator_actor.PrintMessageActor_CannotPrintMessage_Exception`.

Интерфейс:
```
public interface PrintMessageActorWrapper {
    IObject getMessage() throws ReadValueException;
}
```

## get-document-by-id-actor GetDocumentByIdActor GetDocumentByIdActor

Получает документ из базы данных по id.

Если попытка получить документа в коллекцию не удалась, бросает `ru.vp.studgate.get_document_by_id_actor.GetDocumentByIdActor`

Интерфейс:
```
public interface GetDocumentByIdActorWrapper {
    // Получает имя коллекции
    String getCollectionName() throws ReadValueException;
    // Идентификатор документа
    String getEntityId() throws ReadValueException;
    // Имя поля для хранения идентификатора документа в базе данных
    String getIdFieldNameInDatabase() throws ReadValueException;
    // Документ с результатом
    void setDocument(IObject entries) throws ChangeValueException;
}
```
## upsert-session-for-users-actor UpsertSessionForUsersActor UpsertSessionForUsersActor

Ложит пользователя и сессию в один документ.

Если попытка не увенчалась успехом, то вылетит `ru.vp.admin.upsert_session_for_users_actor.UpsertSessionForUsersActorExeption`

Интерфейс:
```
public interface UpsertSessionForUsersActorWrapper {
    // документ для совершения операции
    List<IObject> getDocument() throws ReadValueException;
    // Получает идентификатор сессии
    String getSessionID() throws ReadValueException;
    // Поле для сохранения документа
    void setDocument(IObject doc) throws ChangeValueException;
}
```

## hash-password-create-actor HashPasswordCreateActor HashPasswordCreateActor

Генерирует хеш пароля при содействии BCript`а.

Если что-то не так, то вылетает `ru.vp.admin.hash_password_create_actor.HashPasswordCreateActor_Fail_Exception`

Интерфейс:
```
public interface HashPasswordWrapper {
    // Документ с паролем
    IObject getDocument() throws ReadValueException;
    // Документ с хешем
    void setDocument(IObject result) throws ChangeValueException;
}

```

## get-document-list-by-id-list-actor GetDocumentListByIdListActor GetDocumentListByIdListActor

Получает список документов из базы по id.

Если что-то не так, то вылетает `ru.vp.admin.get_document_list_by_id_list_actor.GetDocumentListByIdListActorException`

Интерфейс:
```
public interface GetDocumentListByIdListActorWrapper {
    // Имя коллекции для поиска
    String getCollectionName() throws ReadValueException;
    // Имя документа
    List<String> getDocumentIds() throws ReadValueException;
    // Имя поля для хранения идентификатора документа в базе данных
    String getIdFieldNameInDatabase() throws ReadValueException;
    //Документ с результатом
    void setDocuments(List<IObject> entries) throws ChangeValueException;
    //Размер страницы выдачи
    String getPageSize() throws ReadValueException;
    //Смешение
    String getPageNumber() throws ReadValueException;
}
```

## create-collection-actor CreateCollectionActor CreateCollectionActor
Актор создаёт коллекцию в базе данных.

Если база не может быть создана, то выбрасываетя  `ru.vp.admin.create_collection_actor.exception.CreateCollectionActorException`

Интерфейс:
```
public interface ICreateCollectionWrapper {
    //Получает имя коллекции которую нужно создать
    String getCollectionName() throws ReadValueException;
}
```

## check-gateway-type-in-payment-method-matrix-actor CheckGatewayTypeInPaymentMethodMatrixActor CheckGatewayTypeInPaymentMethodMatrixActor
Проверяет используется ли метод оплаты в платёжной матрице. 

Если данные не совподают или ошибка в формате,то выбрасываетя  `ru.vp.admin.check_gateway_type_in_payment_method_matrix_actor.CheckGatewayTypeInPaymentMethodMatrixException`

Интерфейс:
```
public interface CheckGatewayTypeInPaymentMethodMatrixActorWrapper {
    
    IObject getGwType() throws ReadValueException;

    List<IObject> getPaymentMatrix() throws ReadValueException;
}
```