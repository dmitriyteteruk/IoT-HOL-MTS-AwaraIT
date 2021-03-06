# Практический тренинг по разработке IoT решений
## Совместное использования технологий Azure, Azure Stack Hub и платформы МТС IoT Hub для "приземления данных" на территории РФ.
В рамках данной практический работы вы научитесь:
- использовать глобальный сервис Azure IoT Hub для удаленной оркестрации контейнерными нагрузками устройства класса Edge;
- считывать данные с сенсоров различного типа и передавать их в платформу МТС IoT Hub;
- считывать данные с сенсоров и передавать их в PaaS сервисы на базе Azure Stack Hub, управляемый МТС, и делать визуализацию с помощью PowerBI.

### Необходимые ресурсы
Для успешного прохождения практической работы вам потребуется:
- учетная запись на платформе Azure Stack Hub (будет предоставлена после подтверждения регистрации);
- учетная запись Azure для использования Azure IoT Hub (участникам будет предоставлен Azure Pass с суммой достаточной для активации сервиса);
- учетная запись на платформе МТС IoT Hub (будет предоставлена после подтверждения регистрации).

### План работы по этапам
#### Развертывание необходимых сервисов для сбора телеметрии
1. Azure:
   1. Активация Azure Pass
   2. [Запуск Azure IoT Hub](https://github.com/dmitriyteteruk/IoT-HOL-MTS-AwaraIT/blob/main/1.2-Setup-Azure-IoT-Hub.md)
   3. [Добавление IoT Edge устройства и конфигурирование приложения](https://github.com/dmitriyteteruk/IoT-HOL-MTS-AwaraIT/blob/main/1.3-AddIoT-Edge-Device-To-Azure-IoT-Hub.md)
2. Azure Stack Hub:
   1. [Создание виртуальной машины (шлюза) Ubuntu 18.04](https://github.com/dmitriyteteruk/IoT-HOL-MTS-AwaraIT/blob/main/2.1-Setup-IoT-Edge-Gateway-VM-ASH.md)
   2. [Установка Azure IoT Edge](https://github.com/dmitriyteteruk/IoT-HOL-MTS-AwaraIT/blob/main/2.2-Setup-Azure-IoT-Edge-Runtime-on-Gateway.md)
   3. [Подключение шлюза к Azure IoT Hub и загрузка приложения](https://github.com/dmitriyteteruk/IoT-HOL-MTS-AwaraIT/blob/main/2.3-Connect-Azure-IoT-Edge-To-IoT-Hub.md)

#### Визуализация полученных данных
4. МТС IoT Hub:
    - Проверка получения данных с IoT Edge устройства
    - Настройка дашборда и предупреждений (email?)
5. Azure Stack Hub и PowerBI:
    - Запуск приложения на базе PaaS сервисов Azure Stack Hub
    - Разработка дашборда на базе PowerBI
