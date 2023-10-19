#### Доступные диплинки в AlfaMobile Android 
| Path| Доступность| Параметры| Примеры| Feature toggles| Экраны| Выкачен в релизе| Примечание |
| /close_account| Внутренний| Параметр - account_number
Параметр - account_name| | | AccountClosingIntroActivity| |  |
| https://online.alfabank.ru/dailypay_account
alfabank://dailypay_account| Внешний| | | Feature.DAILY_PAY_ACCOUNT| AccountDetailsActivity| |  |
| https://online.alfabank.ru/account
alfabank://account| Внешний| Параметр - accountNumber
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - Номер счёта.
Параметр - accountType
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - Тип счёта.
Параметр - shouldOpenRefill
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - Флаг необходимости вызова пополнения счёта при старте экрана.| | | AccountDetailsActivity, AccountDetailsOnWidgetsActivity| 11.39| Открывает экран детализации счёта на виджетах |
| https://online.alfabank.ru/family_account_members
alfabank://family_account_members| Внешний| Параметр - accountNumber| | | AccountMembersActivity| |  |
| /account_rename| Внутренний| Параметр - account_name
Параметр - account_number| | | AccountRenamingActivity| |  |
| /account_requisites| Внутренний| Параметр - account_number
Параметр - account_name| | Feature.ACCOUNT_REQUISITES| AccountRequisitesActivity| |  |
| /account_statements| Внутренний| Параметр - accountNumber
Параметр - productGroup| | Feature.ACCOUNT_STATEMENTS| AccountStatementsActivity| |  |
| /order_statement| Внутренний| Параметр - accountNumber
Параметр - reportType| | Feature.ACCOUNT_STATEMENTS| OrderStatementActivity| |  |
| https://online.alfabank.ru/ready_statements
alfabank://ready_statements| Внешний| Параметр - accountNumber| | Feature.ACCOUNT_STATEMENTS| ReadyStatementsActivity| |  |
| https://online.alfabank.ru/own_accounts_transfer
alfabank://own_accounts_transfer| Внешний| Параметр - currency
Параметр - minor_units
Параметр - amount
Параметр - account_number
Параметр - source_account
Параметр - type| | Feature.CREDIT_PAYMENT_INSUFFICIENT_FUNDS_OWN_TRANSFER, Feature.ME_TO_ME_PULL_IN_ACCOUNT_CARD| AccountToAccountTransferActivity, OwnTransferActivity, PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/conversion
alfabank://conversion| Внешний| Параметр - type| | Feature.MONEY_EXCHANGE| AccountToAccountTransferActivity, OwnTransferActivity, PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/accounts_cards
alfabank://accounts_cards| Внешний| | | | AccountsCardsActivity| |  |
| https://online.alfabank.ru/accounts_opening_details
alfabank://accounts_opening_details| Внешний| Параметр - accountType
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - Тип счёта.
Параметр - conditions
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - Возможное условие открытия счёта.| /accounts_opening_details?accountType=FY
/accounts_opening_details?accountType=FY&conditions=basic
| Feature.ACCOUNTS_OPENING_V2| AccountsOpeningDetailsActivity, OldAccountOpeningDetailsActivity| 11.52| Переход на экран открытия накопительного счёта |
| https://online.alfabank.ru/new_account
alfabank://new_account| Внешний| | /new_account
| | AccountsOpeningActivity| 11.21| Переход на экран выбора типа счёта к открытию |
| /add_external_card| Внутренний| Параметр - shouldShowFinalScreen| | | AddNewCardActivity| |  |
| https://online.alfabank.ru/alfa_check_cards
alfabank://alfa_check_cards| Внешний| | | Feature.ALFA_CHECK_V2| AlfaCheckCardsActivity| |  |
| https://online.alfabank.ru/alfa_check_tariffs
alfabank://alfa_check_tariffs| Внешний| Параметр - cardID
Параметр - cardNumber
Параметр - cardName| | Feature.ALFA_CHECK_V2| AlfaCheckTariffActivity| |  |
| https://online.alfabank.ru/alfa_forex_payment
alfabank://alfa_forex_payment| Внешний| | | Feature.FOREX_PAYMENT_SCREEN| AlfaForexActivity| |  |
| https://online.alfabank.ru/alfa_forex_payment_container
alfabank://alfa_forex_payment_container| Внешний| | | | AlfaForexMainActivity| |  |
| /login_by_qr| Внутренний| Параметр - qrUuid| | Feature.ALFA_ID_QR_AUTH| AlfaIdActivity| |  |
| /alfa_pay_change_card| Внутренний| Параметр - cardId| | Feature.ALFA_PAY_CHANGE_CARD| AlfaPayChangeCardActivity| |  |
| https://online.alfabank.ru/alfa_pay_onboarding| Внешний| | | Feature.ALFA_PAY_ONBOARDING| AlfaPayOnboardingActivity| |  |
| /alfa_pay_card| Внутренний| | | Feature.ALFA_PAY_CARD| AlfaPayCardActivity| |  |
| /alfa_pay_settings| Внутренний| Параметр - cardId| | Feature.ALFA_PAY_SHOW_ACTION_SETTING| AlfaPaySettingsActivity| |  |
| https://online.alfabank.ru/alfa_subscriptions
alfabank://alfa_subscriptions| Внешний| Параметр - subscriptionId| | Feature.ALFA_SUBSCRIPTIONS| AlfaSubscriptionsLandingActivity| |  |
| https://online.alfabank.ru/user_profile/bonuses/alfa_travel
alfabank://user_profile/bonuses/alfa_travel| Внешний| | | Feature.ALFA_TRAVEL_CARD_DETAILS| AlfaTravelActivity| |  |
| https://online.alfabank.ru/profit
alfabank://profit| Внешний| | | Feature.PROFIT| AllBenefitsActivity| |  |
| https://online.alfabank.ru/all_user_products
alfabank://all_user_products| Внешний| | | | AllMyProductsActivity| |  |
| https://online.alfabank.ru/am_app_update
alfabank://am_app_update| Внешний| | | Feature.AM_APP_UPDATE| AppUpdateActivity| |  |
| https://online.alfabank.ru/account_restrictions
alfabank://account_restrictions| Внешний| | | Feature.ACCOUNT_RESTRICTS| ArrestsAndPenaltiesActivity| |  |
| https://online.alfabank.ru/atms
alfabank://atms| Внешний| | | Feature.GEO_INFO, Feature.ATMS_AND_OFFICES_MAP_2020, Feature.YANDEX_MAP, Feature.REDESIGN| AtmsAndOfficesActivity, GeoMapActivity| |  |
| https://online.alfabank.ru/branches
alfabank://branches| Внешний| | | Feature.GEO_INFO, Feature.ATMS_AND_OFFICES_MAP_2020, Feature.YANDEX_MAP, Feature.REDESIGN| AtmsAndOfficesActivity, GeoMapActivity| |  |
| https://online.alfabank.ru/atmsAndBranches
alfabank://atmsAndBranches| Внешний| | | Feature.GEO_INFO, Feature.ATMS_AND_OFFICES_MAP_2020, Feature.REDESIGN, Feature.YANDEX_MAP| AtmsAndOfficesActivity, GeoMapActivity| |  |
| https://online.alfabank.ru/mobile_autopayment
alfabank://mobile_autopayment| Внешний| | | Feature.MOBILE_AUTOPAY_CREATE| SelectContactForAutoPaymentActivity| |  |
| https://online.alfabank.ru/investments/auto_replenishment
alfabank://investments/auto_replenishment| Внешний| Параметр - accountNumber
	- не опцианальное,
	- дефолтное значение - пустая строка.| | Feature.INVESTMENTS_ACCOUNT_REPLENISHMENT_BANNER| AutoPaymentAccountCreateActivity| |  |
| https://online.alfabank.ru/balance_settings
alfabank://balance_settings| Внешний| | | | BalanceSettingsActivity| |  |
| /share| Внутренний| Параметр - text| | Feature.DEEPLINK_SHARE| shareUtils.createShareTextIntent(textToShare, defaultShareTitle)| |  |
| /multistep-route-popup| Внутренний| Параметр - id| | | activityClass| |  |
| /multistep-route-next| Внутренний| Параметр - id
Параметр - stepType
Параметр - skipValidation| | | activityClass| |  |
| https://online.alfabank.ru/transaction_history
alfabank://transaction_history| Внешний| Параметр - searchText
Параметр - account_number
Параметр - mode
Параметр - cardId| | | OperationsHistoryActivity| |  |
| https://online.alfabank.ru/transaction_details
alfabank://transaction_details| Внешний| Параметр - id| | Feature.OPERATIONS_HISTORY| OperationsHistoryDetailsActivity| |  |
| https://online.alfabank.ru/support_chat
alfabank://support_chat| Внешний| Параметр - message| | Feature.CHAT_V3, Feature.BOTTOM_NAVIGATION, Feature.INFO_CHANNELS, Feature.CHAT, Feature.BOTTOM_NAVIGATION, Feature.INFO_CHANNELS| ChatActivity, ChatV3Activity, intent
            .putExtra(EXTRA_NAVIGATION_MENU_SCREEN, mainScreen)
            .putExtra(EXTRA_DEFAULT_CHAT_MESSAGE, defaultMessage)
            .putExtra(EXTRA_SHOULD_REFRESH, shouldRefresh)
            .addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP or Intent.FLAG_ACTIVITY_SINGLE_TOP)| |  |
| https://online.alfabank.ru/user_profile/detail/biom
alfabank://user_profile/detail/biom| Внешний| | | Feature.USER_PROFILE_BIOM_BUTTON| BiometricFlowActivity| |  |
| https://online.alfabank.ru/user_profile/biom
alfabank://user_profile/biom| Внешний| | | Feature.USER_PROFILE_BIOM_BUTTON| BiometricFlowActivity| |  |
| https://online.alfabank.ru/partners_bonus/cashback_history
alfabank://partners_bonus/cashback_history| Внешний| | | Feature.PARTNERS_BONUSES_OFFERS_SUGGESTIONS| BonusesHistoryActivity| |  |
| https://online.alfabank.ru/partners_cashback_longread
alfabank://partners_cashback_longread| Внешний| Параметр - id| | Feature.PARTNERS_BONUSES_OFFERS_SUGGESTIONS| BonusesHistoryLongreadActivity| |  |
| https://online.alfabank.ru/brokerage_withdrawal
alfabank://brokerage_withdrawal| Внешний| Параметр - accountNumber
Параметр - agreementId| | Feature.BROKERAGE_WITHDRAWAL_V2| BrokerageWithdrawalActivity, OldBrokerageWithdrawalActivity| |  |
| /business_account_application| Внутренний| | | Feature.BUSINESS_ACCOUNT_APPLICATION| DynamicMultistepActivity| |  |
| /transaction_history_ul| Внутренний| Параметр - account_number
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 40817810310210087642,
	- описание - Номер счета.| /transaction_history_ul?account_number=40817810310210087642
| Feature.BUSINESS_OPERATIONS_HISTORY| OperationsHistoryActivity| 11.72.00| Диплинк на экран истории операций бизнес счета |
| https://online.alfabank.ru/block_card
alfabank://block_card| Внешний| Параметр - cardId
Параметр - type| | Feature.NEW_CARD_SCREEN, Feature.THIRD_PARTY_NEW_CARD_SCREEN, Feature.NEW_CARD_SCREEN_HOLDER, Feature.NEW_CARD_SCREEN_OWNER| CardBlockingActivity| |  |
| /card_closing| Внутренний| Параметр - cardID| | Feature.NEW_CARD_SCREEN, Feature.THIRD_PARTY_NEW_CARD_SCREEN, Feature.NEW_CARD_SCREEN_HOLDER, Feature.NEW_CARD_SCREEN_OWNER| CardClosingPopupActivity| |  |
| https://online.alfabank.ru/card_delivery
alfabank://card_delivery| Внешний| Параметр - cardId
Параметр - cardType
Параметр - flowType
Параметр - isBonusCard| | Feature.CARD_DELIVERY| CardDeliveryCitiesActivity| |  |
| https://online.alfabank.ru/card_lifecycle_info
alfabank://card_lifecycle_info| Внешний| Параметр - cardId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - идентификатор карты.
Параметр - cardType
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - тип карты.
Параметр - number
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - номер карты.
Параметр - source
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - источник карты.
Параметр - flow
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - признак, по которому идем на экран CardLifecycleActivity (при flow=universal).  +
                    Если параметр flow отсутствует либо не равен universal, тогда идем на экран Информации о доставке.| /card_lifecycle_info?cardId=123
/card_lifecycle_info?cardId=123&cardType=debit&number=1234&source=main
/card_lifecycle_info?cardId=123&cardType=debit&number=1234&source=main&flow=universal
| Feature.CARD_DELIVERY_WIDGET, Feature.CARD_DELIVERY_INFO_YANDEX_MAP, Feature.YANDEX_MAP| CardDeliveryInfoActivity, CardLifecycleActivity, OldCardDeliveryInfoActivity| 11.50| Если выключен фт Feature.CARD_DELIVERY_WIDGET,  +
то не будет осуществлен переход на экран информации о доставке. +
Если в диплинке содержится flow=universal,  +
то будет осуществлен переход на экран CardLifecycleActivity. +
Если параметр cardId отсутствует,  +
то перехода по диплинку не осуществляется, так как для запроса необходим cardId. +
Если включен фт Feature.CARD_DELIVERY_INFO_YANDEX_MAP и YANDEX_MAP,  +
то будет осуществлен переход на экран CardDeliveryInfoActivity. +
Иначе, будет осуществлен переход на экран OldCardDeliveryInfoActivity. |
| /questionnaire| Внутренний| Параметр - product
Параметр - phone| | | WebQuestionnaireActivity| |  |
| https://online.alfabank.ru/cards
alfabank://cards| Внешний| Параметр - id
Параметр - shouldShowContactlessPaymentSystemSnackbar| | Feature.ACCOUNTS_AND_CARDS, Feature.NEW_CARD_SCREEN, Feature.THIRD_PARTY_NEW_CARD_SCREEN, Feature.NEW_CARD_SCREEN_HOLDER, Feature.NEW_CARD_SCREEN_OWNER| CardDetailsActivity, CardDetailsOnWidgetsActivity| |  |
| https://online.alfabank.ru/copy_bonus_number
alfabank://copy_bonus_number| Внешний| Параметр - bonusNumber| | Feature.NEW_CARD_SCREEN| CopyBonusNumberActivity| |  |
| /card_order_third_party| Внутренний| Параметр - alias
	- не опцианальное,
	- дефолтное значение - card-order-alias.
Параметр - fromModule
	- не опцианальное,
	- дефолтное значение - FORM.
Параметр - providerGroupId
	- не опцианальное,
	- дефолтное значение - пустая строка.
Параметр - prefilledDataId
	- не опцианальное,
	- дефолтное значение - пустая строка.| /card_order_third_party?fromModule=FORM&alias=card-order-alias
| Feature.THIRD_PARTY_CARD_ORDER_NATIVE, Feature.KIDS_CARD_ORDER_NATIVE| CardOrderThirdPartyActivity| 11.66| Открывает многошаг заказа карты для третьих лиц, если включен хотя бы один FT из: 
- Feature.THIRD_PARTY_CARD_ORDER_NATIVE;
- Feature.KIDS_CARD_ORDER_NATIVE.

UPD 11.72:
- Добавлены следующие параметры:
- alias,
- fromModule,
- providerGroupId,
- prefilledDataId. |
| /card_refill_selection| Внутренний| Параметр - source
Параметр - destination
Параметр - senderCardsSort
Параметр - recipientCardsSort
Параметр - senderCardId
Параметр - recipientCardId| | Feature.NEW_CARD_SCREEN, Feature.THIRD_PARTY_NEW_CARD_SCREEN, Feature.NEW_CARD_SCREEN_HOLDER, Feature.NEW_CARD_SCREEN_OWNER| CardRefillSelectionActivity| |  |
| https://online.alfabank.ru/card_reissue
alfabank://card_reissue| Внешний| Параметр - isBonusCard
Параметр - name
Параметр - number
Параметр - isLocked
Параметр - isLocked
Параметр - cardId
Параметр - cardType| | Feature.CARD_REISSUE_V2| CardReissueActivity, OldCardReissueActivity| |  |
| https://online.alfabank.ru/account_remapping
alfabank://account_remapping| Внешний| Параметр - cardId| | Feature.NEW_CARD_SCREEN| CardRemappingActivity| |  |
| https://online.alfabank.ru/card_to_savings_account
alfabank://card_to_savings_account| Внешний| Параметр - accountType
Параметр - number
Параметр - amount
Параметр - currency
Параметр - name| | Feature.CARD_TO_SAVINGS_ACCOUNT_TRANSFER| CardToAccountTransferContainerActivity| |  |
| https://online.alfabank.ru/card_to_card
alfabank://card_to_card| Внешний| Параметр - currency
Параметр - minorUnits
Параметр - amount
Параметр - senderCardsSort
Параметр - recipientCardsSort
Параметр - reference
Параметр - cardId
Параметр - isRecipient
Параметр - recipientCardId
Параметр - senderCardId| | Feature.P2P_TRANSFERS, Feature.NEW_P2P, Feature.CARD_TO_CARD_REPEAT_FROM_DEEPLINK| CardToCardTransferContainerActivity, P2PMainActivity, PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/money_pool_transfer
alfabank://money_pool_transfer| Внешний| Параметр - cardId
Параметр - name| | Feature.NEW_P2P, Feature.MONEY_REQUEST| CardToCardTransferContainerActivity, PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/card_to_card_recharge
alfabank://card_to_card_recharge| Внешний| Параметр - recipient_card_id| | Feature.NEW_P2P, Feature.ACCOUNT_DETAILS_ON_WIDGETS| CardToCardTransferContainerActivity, PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/recharge
alfabank://recharge| Внешний| | | | CardToCardTransferContainerActivity, PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/contactless
alfabank://contactless| Внешний| Параметр - id| | | CardTokenizeActivity| |  |
| /card_activation| Внутренний| Параметр - id| | Feature.CARDS_ACTIVATION| CardsActivationActivity| |  |
| https://online.alfabank.ru/user_profile/detail/change_registration_address
alfabank://user_profile/detail/change_registration_address| Внешний| | /user_profile/detail/change_registration_address
| Feature.USER_PROFILE_CHANGE_REGISTRATION_ADDRESS_V2| ChangeActualAddressActivity, OldUserProfileDetailInfoActivity| 11.62| Открывает флоу смены адреса регистрации с картой, если фт выключен то открывает раздел  +
Мои данные в настройках |
| https://online.alfabank.ru/user_profile/change_registration_address
alfabank://user_profile/change_registration_address| Внешний| | /user_profile/change_registration_address
| | ChangeActualAddressActivity| 12.02| Открывает флоу смены адреса регистрации с картой |
| https://online.alfabank.ru/user_profile/detail/change_actual_address
alfabank://user_profile/detail/change_actual_address| Внешний| | /user_profile/detail/change_actual_address
| Feature.USER_PROFILE_CHANGE_ACTUAL_ADDRESS_V2| ChangeActualAddressActivity, OldUserProfileDetailInfoActivity| 11.60| Открывает флоу смены адреса проживания с картой, если фт  +
Feature.USER_PROFILE_CHANGE_ACTUAL_ADDRESS_V2 выключен то открывает раздел Мои данные в настройках |
| https://online.alfabank.ru/user_profile/change_actual_address
alfabank://user_profile/change_actual_address| Внешний| | /user_profile/change_actual_address
| | ChangeActualAddressActivity| 12.02| Открывает флоу смены адреса проживания с картой |
| https://online.alfabank.ru/card_pin_code
alfabank://card_pin_code| Внешний| Параметр - id
Параметр - isAfterTokenization| | | ChangeCardPinActivity| |  |
| /combo_card_longread| Внутренний| | | | ChangeComboCardLimitLongreadActivity| |  |
| https://online.alfabank.ru/credit_cards_limit_management
alfabank://credit_cards_limit_management| Внешний| Параметр - accountNumber
Параметр - type| | | ChangeCreditCardLimitActivity| |  |
| /combo_card_loader| Внутренний| Параметр - infoUrl
Параметр - dataUrl| | | PollingScreenActivity| |  |
| /change_credit_card_limit_confirmation| Внутренний| Параметр - transaction_id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - id транзакции для многошага.| /change_credit_card_limit_confirmation?transaction_id=1234
| Feature.CHANGE_CREDIT_CARD_LIMIT_CONFIRMATION| ChangeCreditCardLimitConfirmationActivity| 12.02| Открывает флоу подтверждения операции для модуля change_credit_card_limit |
| /user_profile/email| Внутренний| | | Feature.USER_PROFILE_CHANGE_EMAIL| ChangeEmailActivity| 12.03| Открывает флоу смены эмейла,
если включен фт Feature.USER_PROFILE_CHANGE_EMAIL для редизайна профиля |
| https://online.alfabank.ru/user_profile/detail/email| Внешний| | | Feature.USER_PROFILE_CHANGE_EMAIL| ChangeEmailActivity, OldUserProfileWidgetActivity| 12.03| Открывает флоу смены эмейла,
если включен фт Feature.USER_PROFILE_CHANGE_EMAIL |
| https://online.alfabank.ru/user_profile/change_passcode
alfabank://user_profile/change_passcode| Внешний| | /user_profile/change_passcode
| Feature.USER_PROFILE_REDESIGN_PASSCODE| ChangePasscodeActivity| 12.02| Если установлен пасскод и включен ФТ USER_PROFILE_REDESIGN_PASSCODE, открывает экран смены пасскода |
| https://online.alfabank.ru/create_new_claim
alfabank://create_new_claim| Внешний| Параметр - branchId| | Feature.CLIENT_CLAIM_FROM_PROFILE| ClaimsMainActivity| |  |
| https://online.alfabank.ru/user_profile/claims_history
alfabank://user_profile/claims_history
https://online.alfabank.ru/claims_history| Внешний| | | Feature.CLAIMS_HISTORY| ClaimsMainActivity| |  |
| alfabank://user_profile/claims_history
https://online.alfabank.ru/claims_history
alfabank://claims_history| Внешний| | | Feature.CLAIMS_HISTORY| ClaimsMainActivity| |  |
| https://online.alfabank.ru/user_profile/claims_history/details
alfabank://user_profile/claims_history/details| Внешний| Параметр - id| | Feature.CLAIMS_HISTORY| ClaimDetailActivity| |  |
| https://online.alfabank.ru/close_combocard
alfabank://close_combocard| Внешний| Параметр - id
Параметр - type| | Feature.COMBO_CARD_CLOSING| ComboCardClosingActivity| |  |
| /info_channels/settings| Внутренний| | | Feature.INFO_CHANNELS_SETTINGS| CommunicationSettingsActivity| |  |
| https://online.alfabank.ru/info_channels
alfabank://info_channels| Внешний| | | Feature.BOTTOM_NAVIGATION, Feature.INFO_CHANNELS| intent
            .putExtra(EXTRA_NAVIGATION_MENU_SCREEN, mainScreen)
            .putExtra(EXTRA_DEFAULT_CHAT_MESSAGE, defaultMessage)
            .putExtra(EXTRA_SHOULD_REFRESH, shouldRefresh)
            .addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP or Intent.FLAG_ACTIVITY_SINGLE_TOP)| |  |
| https://online.alfabank.ru/user_profile/confirm_required
alfabank://user_profile/confirm_required| Внешний| | /user_profile/confirm_required
| Feature.CONFIRM_REQUIRED| ConfirmRequiredActivity| 11.63| Если включен ft Feature.CONFIRM_REQUIRED, откроется экран ConfirmRequiredActivity,\n +
иначе не заходим в фичу |
| https://online.alfabank.ru/user_profile/settings/confirm_required
alfabank://user_profile/settings/confirm_required| Внешний| | /user_profile/settings/confirm_required
| Feature.CONFIRM_REQUIRED| ConfirmRequiredActivity| 11.63| Если включен ft Feature.CONFIRM_REQUIRED, откроется экран ConfirmRequiredActivity,\n +
иначе не заходим в фичу |
| /state-services-sdk-redirect/| Внутренний| Параметр - code
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: eyJ2ZXIiOjEsInR5cCI6IkpXVCIsInNidCI6ImF1dGhvcml6YXRpb25fY29kZSIsImFsZyI6IlJTMjU2In0...,
	- описание - Параметр подставляют Госуслуги. Маркер доступа, полученный у сервиса авторизации ЕСИА  +
                для последующего взаимодействия платформы Цифровый Профиль (нашего бэка) с ЕСИА..
Параметр - error
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: ESIA-910100,
	- описание - Параметр подставляют Госуслуги. Код ошибки на стороне ГУ..
Параметр - error_description
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: В автоматическом режиме не удалось произвести проверку вашего паспорта.,
	- описание - Параметр подставляют Госуслуги. Описание ошибки..| | Feature.SDK_STATE_SERVICES| EmptyStateServicesActivity| 11.72| Открывает экран с повтором запросов, где проверяется, дал ли пользователь согласия на Госуслуги.  +
Данный диплинк вызывается из Мобильного приложения Госуслуг или браузера. ЕСИА не может в диплинке  +
возвращать дополнительные параметры кроме своих, поэтому некоторые данные храняться в статике. |
| https://online.alfabank.ru/connect_state_services
alfabank://connect_state_services| Внешний| Параметр - screenId
Параметр - finalScreenId
Параметр - source| | Feature.CONNECT_STATE_SERVICES| ConnectStateServicesActivity| |  |
| https://online.alfabank.ru/state_services_webview
alfabank://state_services_webview| Внешний| Параметр - screenId
Параметр - finalScreenId
Параметр - source| | Feature.CONNECT_STATE_SERVICES, Feature.SDK_STATE_SERVICES| EsiaStateServicesActivity, StateServicesWebActivity| |  |
| /credit_holidays_bki_check| Внутренний| Параметр - offerId| | | PollingScreenActivity| |  |
| https://online.alfabank.ru/credit_holidays
alfabank://credit_holidays| Внешний| Параметр - account_number
Параметр - offerId| | | CreditHolidaysActivity| |  |
| /credit_holidays_confirm| Внутренний| Параметр - offerId| | | CreditHolidaysConfirmActivity| |  |
| https://online.alfabank.ru/account_information_composite
alfabank://account_information_composite| Внешний| Параметр - account_number| | Feature.CREDIT_INFO_DYNAMIC| CreditInfoActivity| |  |
| https://online.alfabank.ru/annuity-credit/schedule
alfabank://annuity-credit/schedule| Внешний| Параметр - account_number| | Feature.CREDIT_PAYMENT_SCHEDULE| CreditPaymentScheduleActivity| |  |
| https://online.alfabank.ru/credits_and_mortgage
alfabank://credits_and_mortgage| Внешний| | | Feature.CREDIT_WIDGET| CreditsAndMortgageActivity| |  |
| https://online.alfabank.ru/daily_pay_subscribe
alfabank://daily_pay_subscribe| Внешний| Параметр - source| | Feature.DAILY_PAY_SUBSCRIBE| DailyPaymentsSubscribeActivity| |  |
| https://online.alfabank.ru/dashboard/daily_pay/status
alfabank://dashboard/daily_pay/status| Внешний| | | | DailyPaymentsDetailsActivity| |  |
| https://online.alfabank.ru/dailypay_connection_information
alfabank://dailypay_connection_information| Внешний| | | Feature.DAILY_PAY_CONNECTION_INFORMATION| DailyPaymentsConnectionInfoActivity| |  |
| https://online.alfabank.ru/daily_pay_subscribe_sign
alfabank://daily_pay_subscribe_sign| Внешний| | | Feature.DAILY_PAY_SUBSCRIBE| DailyPaymentsSignDocumentsActivity| |  |
| https://online.alfabank.ru/daily_pay_subscribe_verification_pending
alfabank://daily_pay_subscribe_verification_pending| Внешний| | | Feature.DAILY_PAY_SUBSCRIBE| PollingScreenActivity| |  |
| https://online.alfabank.ru/darkModePreferences
alfabank://darkModePreferences| Внешний| | | | DarkModePreferencesActivity| |  |
| https://online.alfabank.ru/debit_card_offers
alfabank://debit_card_offers| Внешний| Параметр - accountNumber
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - Номер счета для запроса предложений.| alfabank:///debit_card_offers/1234
https://online.alfabank.ru/debit_card_offers/1234
| Feature.THIRD_PARTY_CARD_ORDER_NATIVE, Feature.KIDS_CARD_ORDER_NATIVE| CardRecipientOptionsActivity, WebFeatureActivity| 11.65| Открывает экран CardRecipientOptionsActivity, если включен хотя бы один FT из:
- Feature.KIDS_CARD_ORDER_NATIVE;
- Feature.THIRD_PARTY_CARD_ORDER_NATIVE
, иначе открывается старая витрина на webView.

UPD 11.69:
- переименован из /dashboard/debit_card_offers в /debit_card_offers
- открыт публично для хостов alfabank:// и https://online.alfabank.ru |
| https://online.alfabank.ru/debit_card_showcase
alfabank://debit_card_showcase| Внешний| Параметр - flowType
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: SELF, THIRD_PARTY, KIDS,
	- описание - Тип флоу для запроса подходящей витрины.
Параметр - accountNumber
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - Номер счета для запроса подходящей витрины.| alfabank:///debit_card_showcase?flowType=THIRD_PARTY
https://online.alfabank.ru/debit_card_showcase?flowType=KIDS
| Feature.THIRD_PARTY_CARD_ORDER_NATIVE, Feature.KIDS_CARD_ORDER_NATIVE| DebitCardsShowcaseActivity| 11.65| Открывает экран DebitCardsShowcaseActivity, если включен хотя бы один FT из:
- Feature.KIDS_CARD_ORDER_NATIVE;
- Feature.THIRD_PARTY_CARD_ORDER_NATIVE.

UPD 11.69:
- открыт публично для хостов alfabank:// и https://online.alfabank.ru |
| /multicard/setup| Внутренний| Параметр - plasticId
Параметр - funderId
Параметр - cardName
Параметр - cardNumber
Параметр - stage| | Feature.MULTICARD| DecoupledCardFundingCardCategoriesActivity| |  |
| https://online.alfabank.ru/multicard/landing
alfabank://multicard/landing| Внешний| Параметр - cardId| | Feature.MULTICARD| DecoupledCardLandingActivity| |  |
| https://online.alfabank.ru/multicard/setup_card
alfabank://multicard/setup_card| Внешний| Параметр - plasticId
Параметр - stage| | Feature.MULTICARD| DecoupledFundingCardsActivity| |  |
| /multicard/availableCards| Внутренний| | | Feature.MULTICARD| DecoupledCardTransformationActivity| |  |
| /add_to_contacts| Внутренний| Параметр - firstName
Параметр - middleName
Параметр - lastName
Параметр - company
Параметр - job
Параметр - phone
Параметр - email| | Feature.DEEPLINK_ADD_TO_CONTACTS| intentFactory.createIntent().apply {
                action = Intent.ACTION_INSERT
                type = ContactsContract.Contacts.CONTENT_TYPE
                putExtra(Insert.DATA, data)
                putExtra(Insert.COMPANY, company)
                putExtra(Insert.JOB_TITLE, job)
                putExtra(Insert.PHONE, phone)
                putExtra(Insert.EMAIL, email)
            }| |  |
| /deeplink_popup_path| Внутренний| Параметр - endpoint| | Feature.DEEPLINK_POPUP| DeeplinkPopupActivity| |  |
| /partial_deposit_withdrawal| Внутренний| Параметр - accountNumber
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 123232134332,
	- описание - номер счета.| /partial_deposit_withdrawal?accountNumber=2134323432
| | DepositPartialWithdrawalActivity| 12.05| открывает экран частичного снятия с депозитного счета |
| https://online.alfabank.ru/deposits_opening
alfabank://deposits_opening| Внешний| | | | DepositsOpeningActivity| |  |
| https://online.alfabank.ru/user_profile/devices
alfabank://user_profile/devices| Внешний| | /user_profile/devices
| Feature.DEVICE_LIST| DeviceListActivity| 12.02| Если установлен пасскод и включен ФТ Feature.DEVICE_LIST, открывает экран привязанных устройств |
| https://online.alfabank.ru/user_profile/settings/devices
alfabank://user_profile/settings/devices| Внешний| | /user_profile/settings/devices
| Feature.DEVICE_LIST| DeviceListActivity| | Если установлен пасскод и включен ФТ Feature.DEVICE_LIST, открывает экран привязанных устройств |
| https://online.alfabank.ru/user_profile/devices/device
alfabank://user_profile/devices/device| Внешний| Параметр - id| | Feature.DEVICE_STATUS| DeviceStatusActivity| |  |
| https://online.alfabank.ru/user_profile/settings/devices/device
alfabank://user_profile/settings/devices/device| Внешний| Параметр - id| | Feature.DEVICE_STATUS| DeviceStatusActivity| |  |
| /marketplace/marketplace_insurance| Внутренний| Параметр - url| | Feature.MARKETPLACE_INSURANCE| DigitalInsuranceActivity, WebFeatureActivity| |  |
| alfabank://user_profile/digital_ticket
https://online.alfabank.ru/digital_ticket
alfabank://digital_ticket| Внешний| | | Feature.DIGITAL_TICKET| DigitalTicketActivity| |  |
| https://online.alfabank.ru/user_profile/digital_ticket
alfabank://user_profile/digital_ticket
https://online.alfabank.ru/digital_ticket| Внешний| | | Feature.DIGITAL_TICKET| DigitalTicketActivity| |  |
| https://online.alfabank.ru/incomplete_operations/sign_operation_at_branch
alfabank://incomplete_operations/sign_operation_at_branch| Внешний| Параметр - id| | Feature.SIGN_ONLINE_IN_UNAPPROVED| DocumentSigningSessionActivity| |  |
| /documents_state_services| Внутренний| | | Feature.DOCUMENTS_STATE_SERVICES| DocumentsStateServicesActivity| |  |
| /document_details_state_services| Внутренний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: Passport-1169894143,
	- описание - id документа.| /document_details_state_services?id=Passport-1169894143
| Feature.DOCUMENTS_STATE_SERVICES| DocumentDetailsStateServicesActivity| 12.02| Открывает экран деталки документа, если указан его id |
| https://online.alfabank.ru/longread
alfabank://longread| Внешний| Параметр - endpoint| | | DownloadingLongreadActivity| |  |
| /dynamic_fields_bottom_sheet| Внутренний| Параметр - screen
Параметр - alias
Параметр - screenTitle
Параметр - shouldCloseOnAction| | Feature.DYNAMIC_FIELDS_BOTTOM_SHEET| DeeplinkDynamicFieldsBottomSheetActivity| |  |
| https://online.alfabank.ru/user_profile/detail/passport_intro
alfabank://user_profile/detail/passport_intro| Внешний| | | Feature.USER_PASSPORT_UPDATE| IntroPassportActivity| |  |
| /user_profile/detail/passport_intro/update_reasons| Внутренний| | | Feature.USER_PASSPORT_UPDATE| ChooseReasonActivity| |  |
| https://online.alfabank.ru/user_profile/detail/phone_numbers_change_request
alfabank://user_profile/detail/phone_numbers_change_request| Внешний| | | Feature.CHANGE_PHONE_NUMBERS| EditPhoneCancelActivity| |  |
| https://online.alfabank.ru/user_profile/phone_numbers
alfabank://user_profile/phone_numbers| Внешний| | | Feature.CHANGE_PHONE_NUMBERS| EditPhoneActivity| |  |
| https://online.alfabank.ru/user_profile/detail/phone_numbers
alfabank://user_profile/detail/phone_numbers| Внешний| | | Feature.CHANGE_PHONE_NUMBERS| EditPhoneActivity| |  |
| https://online.alfabank.ru/enriched_operation
alfabank://enriched_operation| Внешний| Параметр - id| | | EnrichedOperationActivity, NotificationCenterActivity| |  |
| https://online.alfabank.ru/currency_rates
alfabank://currency_rates| Внешний| Параметр - showcaseMetal
Параметр - endpoint| | Feature.METAL_SHOWCASE, Feature.EXCHANGE_CURRENCY| ExchangeCurrencyActivity, MetalExchangeShowcaseActivity| |  |
| /tel| Внутренний| Параметр - number
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - номер телефона (поле необходимо кодировать).| /tel?number=112
/tel?number=%2B7%20%28900%29-999-11-22
| | intentFactory.createIntent()
            .apply {
                action = Intent.ACTION_DIAL
                data = Uri.parse(TEL_SCHEME + phoneNumber)
            }
            .takeIf { it.resolveActivity(packageManager) != null }| 11.72| Если в системе есть приложение для обработки экшена Intent.ACTION_DIAL,  +
то открывает это приложение с предзаполненным номером телефона, иначе ничего не делает |
| /mailto| Внутренний| Параметр - email
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - почтовый адрес.
Параметр - subject
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - тема письма.| /mailto?email=pochta%40mail.ru
/mailto?email=pochta%40mail.ru&subject=Hello%20world
| | intentFactory.createIntent()
            .apply {
                action = Intent.ACTION_SENDTO
                data = Uri.parse(MAIL_TO_SCHEME)
                putExtra(Intent.EXTRA_EMAIL, arrayOf(email))
                putExtra(Intent.EXTRA_SUBJECT, subject)
            }
            .takeIf { it.resolveActivity(packageManager) != null }| 11.72| Если в системе есть приложение для обработки экшена Intent.ACTION_SENDTO,  +
то открывает это приложение с предзаполненными полями для email и темы сообщения, иначе ничего не делает |
| https://online.alfabank.ru/user_profile/fraud_report
alfabank://user_profile/fraud_report| Внешний| | | Feature.FRAUD_REPORT_DEEPLINK| FraudReportActivity| |  |
| https://online.alfabank.ru/global_search
alfabank://global_search| Внешний| Параметр - PARAM_SCREEN
Параметр - PARAM_RESULT_ID
Параметр - PARAM_QUERY| | Feature.GLOBAL_SEARCH| GlobalSearchActivity| |  |
| https://online.alfabank.ru/investbox_percent_purchase
alfabank://investbox_percent_purchase| Внешний| Параметр - accountNumber| | Feature.OPEN_INVESTBOX| GoalsManagementPurchasesPercentageActivity| |  |
| /goals| Внутренний| | | | GoalsManagementOnboardingActivity| |  |
| https://online.alfabank.ru/goals/refill_settings
alfabank://goals/refill_settings| Внешний| Параметр - accountNumber
Параметр - isNewGoal| | | GoalsManagementSettingsActivity| |  |
| https://online.alfabank.ru/imsi_confirmation
alfabank://imsi_confirmation| Внешний| | | Feature.IMSI_CONFIRM| ImsiConfirmationActivity| |  |
| https://online.alfabank.ru/credit_payment_schedule
alfabank://credit_payment_schedule| Внешний| Параметр - account| | Feature.INSTALLMENT_CARD_REPAYMENT_SCHEDULE| InstallmentCardRepaymentScheduleActivity| |  |
| https://online.alfabank.ru/instalments/new_instalment
alfabank://instalments/new_instalment| Внешний| Параметр - source| | Feature.CREDIT_CARDS_PLAN_IT| InstalmentLoanPlanActivity| |  |
| https://online.alfabank.ru/instalments/loan_detail
alfabank://instalments/loan_detail| Внешний| Параметр - id
Параметр - type
Параметр - agreementNumber| | Feature.CREDIT_CARDS_PLAN_IT, Feature.DEBIT_INSTALLMENT| InstalmentLoanDetailsActivity| |  |
| https://online.alfabank.ru/instalments/new_debit_instalment
alfabank://instalments/new_debit_instalment| Внешний| Параметр - source
Параметр - amount
Параметр - id| | Feature.DEBIT_INSTALLMENT| PlanDebitActivity.createIntent(context, source, amount, operationId)| |  |
| https://online.alfabank.ru/instalments
alfabank://instalments| Внешний| Параметр - source| | Feature.CREDIT_CARDS_PLAN_IT, Feature.DEBIT_INSTALLMENT| InstalmentLoansActivity| |  |
| https://online.alfabank.ru/debit_recalculation
alfabank://debit_recalculation| Внешний| Параметр - source
Параметр - offerId| | Feature.DEBIT_INSTALLMENT_RECALCULATION| DebitRecalculationActivity| |  |
| https://online.alfabank.ru/swift_transfer
alfabank://swift_transfer| Внешний| | | Feature.SWIFT_TRANSFER| InternationalTransferByRequisitesActivity| |  |
| https://online.alfabank.ru/autoaccumulation_settings
alfabank://autoaccumulation_settings| Внешний| Параметр - accountNumber| | Feature.OPEN_INVESTBOX| InvestboxAutoReplenishmentActivity| |  |
| /redirect_to_ai| Внутренний| Параметр - link| | | InvestmentsAppRedirectActivity| |  |
| https://online.alfabank.ru/assets_overview
alfabank://assets_overview| Внешний| Параметр - type
Параметр - category
Параметр - currency| | | AssetsOverviewActivity, CategoryOverviewActivity| |  |
| https://online.alfabank.ru/investments/portfolio
alfabank://investments/portfolio| Внешний| | | | AssetsOverviewActivity| |  |
| https://online.alfabank.ru/investments/catalogue
alfabank://investments/catalogue| Внешний| Параметр - tab| | | InvestmentsCatalogueActivity| |  |
| https://online.alfabank.ru/investments/cross_auth
alfabank://investments/cross_auth| Внешний| | | | InvestmentsCrossAuthorizationActivity| |  |
| https://online.alfabank.ru/investments/showcase/security_details
alfabank://investments/showcase/security_details| Внешний| Параметр - securityId| | | FinancialAssetCatalogueDetailsActivity| |  |
| https://online.alfabank.ru/investments/forecast
alfabank://investments/forecast| Внешний| Параметр - isin
Параметр - title
Параметр - subtitle
Параметр - url| | | InvestmentsForecastActivity| |  |
| https://online.alfabank.ru/investments/instrument_collections
alfabank://investments/instrument_collections| Внешний| Параметр - endpoint| | | InvestmentsInstrumentCollectionsActivity| |  |
| https://online.alfabank.ru/investments/catalog_types
alfabank://investments/catalog_types| Внешний| | | | InvestmentsInstrumentsActivity| |  |
| https://online.alfabank.ru/investments/insurance/order-fields
alfabank://investments/insurance/order-fields| Внешний| Параметр - id| | | InvestmentsLifeInsuranceBuyingFlowActivity| |  |
| https://online.alfabank.ru/investments/insurance
alfabank://investments/insurance| Внешний| Параметр - id| | | InvestmentsLifeInsuranceProductCardActivity| |  |
| https://online.alfabank.ru/investments/insurance/policy
alfabank://investments/insurance/policy| Внешний| Параметр - id| | | InvestmentsLifeInsurancePolicyCardActivity| |  |
| https://online.alfabank.ru/investments/market_asset_card
alfabank://investments/market_asset_card| Внешний| Параметр - url
Параметр - id
Параметр - type
Параметр - title
Параметр - subtitle| | Feature.INVESTMENTS_MARKET_ASSET_CARD| InvestmentsMarketAssetCardActivity| |  |
| https://online.alfabank.ru/investments/market_asset_card/purchase
alfabank://investments/market_asset_card/purchase| Внешний| Параметр - id
Параметр - fromScreen
Параметр - sumValue| | Feature.INVESTMENTS_MARKET_ASSET_PURCHASE| InvestmentsMarketAssetPurchaseActivity| |  |
| https://online.alfabank.ru/investments/popular_instruments
alfabank://investments/popular_instruments| Внешний| Параметр - endpoint| | | InvestmentsPenchantsActivity| |  |
| https://online.alfabank.ru/investments/primary_bonds_placement
alfabank://investments/primary_bonds_placement| Внешний| Параметр - actionType
Параметр - id
Параметр - id| | Feature.INVESTMENTS_PRIMARY_BONDS_PLACEMENT| OpenInvestmentsAccountActivity, PrimaryBondPlacementDetailsActivity, PrimaryBondPlacementPurchaseActivity, PrimaryBondsPlacementCatalogueActivity| |  |
| https://online.alfabank.ru/investments_recommendation_purchase
alfabank://investments_recommendation_purchase| Внешний| Параметр - fromScreen| | Feature.INVESTMENTS_RECOMMENDATION_PURCHASE| InvestmentsRecommendationPurchaseActivity| |  |
| /invoice| Внутренний| Параметр - reference| | | InvoicePaymentActivity| |  |
| https://online.alfabank.ru/knowledge_base/articles_list
alfabank://knowledge_base/articles_list| Внешний| Параметр - id| | Feature.KNOWLEDGE_BASE_FEATURE| KnowledgeBaseArticlesActivity| |  |
| https://online.alfabank.ru/knowledge_base_articles_list
alfabank://knowledge_base_articles_list| Внешний| Параметр - id| | Feature.KNOWLEDGE_BASE_FEATURE| KnowledgeBaseArticlesActivity| |  |
| https://online.alfabank.ru/knowledge_base_article
alfabank://knowledge_base_article| Внешний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: Perevody_v_rubljah,
	- описание - id статьи в базе знаний.| /knowledge_base/article
/knowledge_base/article?id=Perevody_v_rubljah
| Feature.KNOWLEDGE_BASE_FEATURE| KnowledgeBaseLongreadActivity| 11.38| Открывает экран статьи базы знаний,
если включен фт Feature.KNOWLEDGE_BASE_FEATURE |
| https://online.alfabank.ru/knowledge_base/article
alfabank://knowledge_base/article| Внешний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: Perevody_v_rubljah,
	- описание - id статьи в базе знаний.| /knowledge_base_article
/knowledge_base_article?id=Perevody_v_rubljah
| Feature.KNOWLEDGE_BASE_FEATURE| KnowledgeBaseLongreadActivity| 11.38| Открывает экран статьи базы знаний,
если включен фт Feature.KNOWLEDGE_BASE_FEATURE |
| https://online.alfabank.ru/knowledge_base
alfabank://knowledge_base| Внешний| | /knowledge_base
| Feature.KNOWLEDGE_BASE_FEATURE| KnowledgeBaseMainActivity| 11.38| Открывает экран с темами базы знаний,
если включен фт Feature.KNOWLEDGE_BASE_FEATURE |
| https://online.alfabank.ru/limits
alfabank://limits| Внешний| | | Feature.AML_SERVICE| LimitsActivity, OldLimitsActivity| |  |
| https://online.alfabank.ru/
https://platiqr.ru/| Внешний| Параметр - refresh| | Feature.WIDGET_DASHBOARD, Feature.BOTTOM_NAVIGATION| intent
            .putExtra(EXTRA_NAVIGATION_MENU_SCREEN, mainScreen)
            .putExtra(EXTRA_DEFAULT_CHAT_MESSAGE, defaultMessage)
            .putExtra(EXTRA_SHOULD_REFRESH, shouldRefresh)
            .addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP or Intent.FLAG_ACTIVITY_SINGLE_TOP)| |  |
| https://online.alfabank.ru/user_profile/commissions
alfabank://user_profile/commissions| Внешний| | | Feature.JUST_READ_THE_COMMISSIONS| MarkdownViewerActivity| |  |
| /markdown_viewer| Внутренний| Параметр - endpoint| | | MarkdownViewerActivity| |  |
| https://online.alfabank.ru/marketplace
alfabank://marketplace| Внешний| | | Feature.BOTTOM_NAVIGATION| intent
            .putExtra(EXTRA_NAVIGATION_MENU_SCREEN, mainScreen)
            .putExtra(EXTRA_DEFAULT_CHAT_MESSAGE, defaultMessage)
            .putExtra(EXTRA_SHOULD_REFRESH, shouldRefresh)
            .addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP or Intent.FLAG_ACTIVITY_SINGLE_TOP)| |  |
| https://online.alfabank.ru/me2me_push
alfabank://me2me_push| Внешний| Параметр - ref| | Feature.ME_TO_ME_NEW_FINAL_SCREENS_ANDROID, Feature.ME_TO_ME_PUSH| MeToMeTransferConfirmationActivity| |  |
| /settings/me_to_me_auto_accept| Внутренний| | | Feature.ME_TO_ME_NEW_FINAL_SCREENS_ANDROID| MeToMeAutoAcceptActivity| |  |
| https://online.alfabank.ru/settings/external_phone_transfer
alfabank://settings/external_phone_transfer| Внешний| | | Feature.PHONE_EXTERNAL_TRANSFER_SETTINGS| PhoneTransferInfoActivity, PhoneTransferInfoRedesignActivity| |  |
| https://online.alfabank.ru/phone_bank_transfers
alfabank://phone_bank_transfers| Внешний| Параметр - account_number| | Feature.NEW_MOBILE_PHONE_TRANSFER| MobilePhoneTransferActivity, PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/mobile_payment
alfabank://mobile_payment| Внешний| Параметр - phoneNumber| | | MobileRechargeActivity| |  |
| /create_money_request| Внутренний| | | Feature.MONEY_REQUEST| ChooseMoneyRequestCategoryActivity| |  |
| https://online.alfabank.ru/mortgage_insurance
alfabank://mortgage_insurance| Внешний| Параметр - accountNumber
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - номер ипотечного счета, по которому производится фильтрация полисов для отображения.| /mortgage_insurance?accountNumber=40817810604880000891
| Feature.MORTGAGE_INSURANCE| MortgageInsuranceActivity| 11.67| Диплинк для перехода на экран со списком ипотечных полисов |
| https://online.alfabank.ru/mortgage_insurance_exp_policies
alfabank://mortgage_insurance_exp_policies| Внешний| | /mortgage_insurance_exp_policies
| Feature.MORTGAGE_INSURANCE| MortgageInsuranceActivity| 11.73| Универсальный диплинк для перехода на экран со списком ипотечных полисов для пролонгации |
| /mortgage_insurance_info| Внутренний| Параметр - policyId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - id страхового полиса.| /mortgage_insurance_info?policyId=03432%2F118%2F13030325
| | MortgageInsuranceDetailsActivity| 11.67| Диплинк для перехода на экран с информацией о статусе платежа по пролонгации ипотечного полиса |
| /mortgage_insurance_multistep| Внутренний| Параметр - providerGroupId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - id провайдера.
Параметр - prefilledDataId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - id страхового полиса.| /mortgage_insurance_multistep
            ?providerGroupId=08882_7713056834_insurance
            &prefilledDataId=03432%2F118%2F13030325
| | MortgageInsuranceMultistepActivity| 11.67| Диплинк для перехода на экран многошага с пролонгацией ипотечного полиса |
| https://online.alfabank.ru/update_investment_autopayment
alfabank://update_investment_autopayment| Внешний| Параметр - template_id
Параметр - template_route_id| | Feature.TEMPLATES_REDESIGN| EditTemplateActivity| |  |
| https://online.alfabank.ru/create_investment_autopayment
alfabank://create_investment_autopayment| Внешний| Параметр - reference| | | CreateTemplateActivity| |  |
| https://online.alfabank.ru/delete_external_card_dialog
alfabank://delete_external_card_dialog| Внешний| Параметр - cardId
Параметр - shortNumber
Параметр - name| | Feature.EXTERNAL_CARDS_VIEW| DeeplinkDialogActivity| |  |
| https://online.alfabank.ru/non_client_card_order
alfabank://non_client_card_order| Внешний| Параметр - action| | Feature.NON_CLIENT_U0, Feature.NON_CLIENT_NI| NonClientCardOrderActivity| |  |
| https://online.alfabank.ru/non_client_debet_alfa_card_anket
alfabank://non_client_debet_alfa_card_anket| Внешний| Параметр - phone| | | NonClientDebitFormActivity| |  |
| /non_client_change_identification_in_progress| Внутренний| | | Feature.NON_CLIENT_U0, Feature.NON_CLIENT_NI| NonClientLimitsCheckInProgressDeeplinkDialogActivity| |  |
| /non_client_upgrade_to_simple_identification| Внутренний| | | Feature.NON_CLIENT_U0, Feature.NON_CLIENT_NI| NonClientLimitsInfoActivity| |  |
| https://online.alfabank.ru/non_client_limit
alfabank://non_client_limit| Внешний| | | Feature.NON_CLIENT_U0, Feature.NON_CLIENT_NI| NonClientLimitsActivity| |  |
| /non_client_showcase_detailed| Внутренний| Параметр - phone_number
Параметр - product_code| | | NonClientsShowcaseDetailsActivity| |  |
| https://online.alfabank.ru/user_profile/settings/ofd
alfabank://user_profile/settings/ofd| Внешний| | | Feature.OFD_RECEIPTS| OfdSettingsActivity| 11.51| Открывает экран на подключение отображения чеков в истории операций,
если включен фт Feature.OFD_RECEIPTS |
| https://online.alfabank.ru/user_profile/ofd
alfabank://user_profile/ofd| Внешний| | | Feature.OFD_RECEIPTS| OfdSettingsActivity| 11.51| Открывает экран на подключение отображения чеков в истории операций,
если включен фт Feature.OFD_RECEIPTS |
| https://online.alfabank.ru/user_profile/settings/statements_order
alfabank://user_profile/settings/statements_order| Внешний| | | Feature.STATEMENT_ORDER_WEBVIEW| WebFeatureActivity| |  |
| https://online.alfabank.ru/user_profile/settings
alfabank://user_profile/settings| Внешний| | | Feature.WIDGET_USER_PROFILE| OldAppPreferencesActivity| |  |
| https://online.alfabank.ru/investments/invest_idea
alfabank://investments/invest_idea| Внешний| Параметр - id| | Feature.INVESTMENTS_RECOMMENDATIONS| InvestIdeaActivity| |  |
| https://online.alfabank.ru/investments
alfabank://investments| Внешний| | | | InvestmentsMainActivity| |  |
| https://online.alfabank.ru/info_channels/notifications_channel
alfabank://info_channels/notifications_channel| Внешний| | | Feature.NOTIFICATIONS_CHANNEL, Feature.NOTIFICATION_CENTER| NotificationCenterActivity, NotificationsChannelActivity| |  |
| https://online.alfabank.ru/notification_center
alfabank://notification_center| Внешний| Параметр - notification_type| | Feature.NOTIFICATION_CENTER, Feature.NOTIFICATIONS_CHANNEL| NotificationCenterActivity, NotificationsChannelActivity| |  |
| https://online.alfabank.ru/payments_hub
alfabank://payments_hub| Внешний| | | Feature.BOTTOM_NAVIGATION, Feature.BOTTOM_NAVIGATION_FOR_THIRD_PARTY_CLIENT| AllPaymentsActivity, intent
            .putExtra(EXTRA_NAVIGATION_MENU_SCREEN, mainScreen)
            .putExtra(EXTRA_DEFAULT_CHAT_MESSAGE, defaultMessage)
            .putExtra(EXTRA_SHOULD_REFRESH, shouldRefresh)
            .addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP or Intent.FLAG_ACTIVITY_SINGLE_TOP)| |  |
| https://online.alfabank.ru/add_expense
alfabank://add_expense| Внешний| | | Feature.PFM| OldPfmWebActivity| |  |
| https://online.alfabank.ru/user_profile/cash_order
alfabank://user_profile/cash_order| Внешний| | | Feature.CASH_ORDER| WebFeatureActivity| |  |
| https://online.alfabank.ru/user_profile/detail
alfabank://user_profile/detail| Внешний| | | | OldUserProfileDetailInfoActivity.createIntent(context)| |  |
| /onboarding_widget_article| Внутренний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - идентификатор статьи в базе знаний.
Параметр - productType
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: CT_CLIENT_CARD,
	- описание - тип продукта.
Параметр - stepId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - id шага.
Параметр - stepName
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - название шага.
Параметр - stepStatus
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: NEW, IN_PROGRESS, DONE, LOCKED,
	- описание - статус шага.| /onboarding_widget_article?id=0
/onboarding_widget_article?id=0&productType=CT_CLIENT_CARD
/onboarding_widget_article?id=0&productType=CT_CLIENT_CARD&stepId=0
/onboarding_widget_article?id=0&productType=CT_CLIENT_CARD&stepId=0&stepName=name
/onboarding_widget_article?id=0&productType=CT_CLIENT_CARD&stepId=0&stepName=name&stepStatus=NEW
| Feature.ONBOARDING_WIDGET| OnboardingArticleActivity| 11.54| Открывает экран статьи виджита онбоардинга,
если включен фт Feature.ONBOARDING_WIDGET |
| https://online.alfabank.ru/investments/open_investments_account
alfabank://investments/open_investments_account| Внешний| Параметр - type
Параметр - shouldRouteToInvestments| | Feature.OPEN_INVEST_ACCOUNT, Feature.OPEN_BROKERAGE_ACCOUNT_REDESIGN, Feature.OPEN_INVESTBOX, Feature.INVEST_BOX_OPENING_REDESIGNED| OpenInvestmentsAccountActivity, OpenInvestmentsAccountRedesignedActivity| |  |
| https://online.alfabank.ru/investments/open_brokerage_account
alfabank://investments/open_brokerage_account| Внешний| | | Feature.OPEN_BROKERAGE_ACCOUNT_REDESIGN| OpenInvestmentsAccountActivity| |  |
| https://online.alfabank.ru/open_new_product
alfabank://open_new_product| Внешний| | | Feature.OPEN_NEW_PRODUCT_V2| OpenNewProductActivity| |  |
| https://online.alfabank.ru/loyalty_compensation
alfabank://loyalty_compensation| Внешний| Параметр - loyaltyType
Параметр - title| | Feature.LOYALTY_COMPENSATION| OperationCompensationActivity| |  |
| https://online.alfabank.ru/overall_loyalty
alfabank://overall_loyalty| Внешний| Параметр - type
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - тип предвыбранного счёта.| /overall_loyalty?type=104
| | OverallLoyaltyActivity| 11.40| Открывает экран Весь Ваш Кешбек
Если параметр type не приходит, на экране отобразится первый счёт из списка |
| https://online.alfabank.ru/partner_bonus_instruction
alfabank://partner_bonus_instruction| Внешний| | | Feature.PARTNER_BONUS_INSTRUCTION| PartnerBonusInstructionActivity| |  |
| https://online.alfabank.ru/partners_bonus
alfabank://partners_bonus| Внешний| Параметр - title| | Feature.PARTNERS_BONUSES_OFFERS_SUGGESTIONS, Feature.PARTNERS_BONUSES| PartnersBonusesActivity, PartnersBonusesMainActivity, PartnersBonusesThematicMainActivity| |  |
| https://online.alfabank.ru/partners_bonuses_for_category
alfabank://partners_bonuses_for_category| Внешний| Параметр - id
Параметр - title| | Feature.PARTNERS_BONUSES_WITH_WIDGETS| PartnersBonusesActivity| |  |
| https://online.alfabank.ru/partners_bonus/partners_bonuses_for_categories
alfabank://partners_bonus/partners_bonuses_for_categories| Внешний| Параметр - title| | Feature.PARTNERS_BONUSES| BonusCategoriesActivity| |  |
| https://online.alfabank.ru/partners_bonus_details
alfabank://partners_bonus_details| Внешний| Параметр - id| | Feature.PARTNERS_BONUSES, Feature.PARTNERS_BONUSES_DETAILS_DATAVIEW_VERSION| PartnersBonusDetailsActivity, PartnersBonusDetailsRedesignActivity| |  |
| https://online.alfabank.ru/external_transfer_by_bic
alfabank://external_transfer_by_bic| Внешний| Параметр - id
Параметр - from| | Feature.PAYMENT_TRANSFER_CONTAINER| PaymentTransferContainerActivity| |  |
| https://online.alfabank.ru/gosuslugi
alfabank://gosuslugi| Внешний| | | Feature.GOS_PAYMENTS| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/communal_subscription
alfabank://communal_subscription| Внешний| | | Feature.DYNAMIC_PAYMENT_COMMUNAL| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/transport_payment
alfabank://transport_payment| Внешний| | | Feature.TRANSPORT_DYNAMIC_FIELDS, Feature.TRANSPORT_PAYMENTS, Feature.CATALOG_PAYMENTS| CatalogueSearchActivity, PaymentsSearchActivity| |  |
| https://online.alfabank.ru/externalcredit_payment
alfabank://externalcredit_payment| Внешний| | | Feature.EXTERNAL_CREDIT_DYNAMIC_FIELDS| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/charity_payment
alfabank://charity_payment| Внешний| | | | PaymentsSearchActivity| |  |
| https://online.alfabank.ru/internet_payment
alfabank://internet_payment| Внешний| | | Feature.INTERNET_DYNAMIC, Feature.INTERNET_PAYMENTS| CatalogueSearchActivity, PaymentsSearchActivity| |  |
| https://online.alfabank.ru/providers_search
alfabank://providers_search| Внешний| Параметр - type
Параметр - category| | Feature.INVOICE_DASHBOARD_V2| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/emoney_payment
alfabank://emoney_payment| Внешний| | | Feature.EMONEY_DYNAMIC_FIELDS| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/education
alfabank://education| Внешний| | | Feature.EDUCATION_DYNAMIC_FIELDS| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/games
alfabank://games| Внешний| | | Feature.GAMES_DYNAMIC_FIELDS| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/all_providers_search
alfabank://all_providers_search| Внешний| | | Feature.WIDGET_PAYMENT_HUB_SEARCH_BUTTON| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/other_payment
alfabank://other_payment| Внешний| | | Feature.OTHER_DYNAMIC_FIELDS| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/providers
alfabank://providers| Внешний| Параметр - type
Параметр - title
Параметр - searchPlaceholder
Параметр - feature
Параметр - qrFeatureToggle| | Feature.values()| PaymentsSearchActivity| |  |
| https://online.alfabank.ru/pdf_viewer
alfabank://pdf_viewer| Внешний| Параметр - url
Параметр - title
Параметр - type| | Feature.PDF_VIEWER| Intent.createChooser(targetIntent, pdfTitle), PdfViewerActivity| |  |
| https://online.alfabank.ru/pension_transfer
alfabank://pension_transfer| Внешний| | | Feature.PENSION_TRANSFER| PensionTransferActivity| |  |
| /pension_transfer_from_uzesia| Внутренний| Параметр - status
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: SUCCESSFUL, PROCESSING, FAILED,
	- описание - Статус подтверждённости УЗ на портале ЕСИА..| /pension_transfer_from_uzesia?status=SUCCESSFUL
| Feature.PENSION_TRANSFER_FROM_UZESIA| PensionTransferFromUzEsiaActivity| 12.03| Диплинк необходим для отправки статуса на мидл и получения дальнейшего диплинка  +
(на продолжение фичи или возврат на главный экран). +
Если включен FT PENSION_TRANSFER_FROM_UZESIA, откроется экран PensionTransferFromUzEsiaActivity. |
| https://online.alfabank.ru/personal_finance_advisor| Внешний| | | Feature.PERSONAL_FINANCE_ADVISOR| PfaLandingActivity| |  |
| https://online.alfabank.ru/pfm
alfabank://pfm| Внешний| Параметр - page
Параметр - cardid
Параметр - accountNumber| | Feature.PFM_V3, Feature.PFM| OldPfmMainActivity, PfmMainActivity| |  |
| /polling| Внутренний| Параметр - infoUrl
Параметр - dataUrl| | | PollingScreenActivity| |  |
| /portrait_video| Внутренний| Параметр - button_text
Параметр - button_deeplink
Параметр - button_start_time
Параметр - resize_mode
Параметр - video_url
Параметр - loop
Параметр - pip_mode| | Feature.PORTRAIT_VIDEO| PortraitVideoPlayerActivity| 11.55.00| Если включен ft Feature.PORTRAIT_VIDEO и все обязательные параметры,
откроется новый экран PortraitVideoPlayerActivity,
иначе ничего не открывается |
| https://online.alfabank.ru/alfa_premium_showcase
alfabank://alfa_premium_showcase| Внешний| | | Feature.ALFA_PREMIUM| PremiumActivity| |  |
| https://online.alfabank.ru/simplewine
alfabank://simplewine| Внешний| | | Feature.SIMPLEWINE| PremiumBonusActivity| |  |
| https://online.alfabank.ru/restaurants_compensations
alfabank://restaurants_compensations| Внешний| | | Feature.PREMIUM_AIRPORT_RESTAURANTS_REFUND| AirportRestaurantsRefundActivity| |  |
| https://online.alfabank.ru/alfa_premium_levels
alfabank://alfa_premium_levels| Внешний| | | Feature.ALFA_PREMIUM_LEVELS| PremiumLevelsActivity| |  |
| https://online.alfabank.ru/premium_service_ad
alfabank://premium_service_ad| Внешний| Параметр - from
Параметр - media_source
Параметр - campaign| | Feature.PREMIUM_SERVICE_AD| PremiumServiceAdActivity| |  |
| https://online.alfabank.ru/user_profile/bonuses/priority_pass
alfabank://user_profile/bonuses/priority_pass| Внешний| | | Feature.BONUS_AVAILABLE| BonusDetailsActivity| |  |
| https://online.alfabank.ru/private_coins
alfabank://private_coins| Внешний| | | Feature.ALFA_PRIVATE_COINS| PrivateCoinsActivity| |  |
| https://online.alfabank.ru/account_details_on_widgets
alfabank://account_details_on_widgets| Внешний| Параметр - accountNumber
Параметр - url| | Feature.CREDIT_SCREEN| ProductDetailsActivity| |  |
| https://online.alfabank.ru/linelife
alfabank://linelife| Внешний| | | | ProviderPaymentActivity| |  |
| https://online.alfabank.ru/fssp
alfabank://fssp| Внешний| | | Feature.GOS_PAYMENTS| ProviderPaymentActivity| |  |
| https://platiqr.ru/| Внешний| | | | ProviderPaymentActivity| |  |
| /show_provider_multistep_popup| Внутренний| Параметр - id| | Feature.PROVIDER_MULTISTEP_POPUP| activityClass| |  |
| https://online.alfabank.ru/gibdd
alfabank://gibdd| Внешний| | | Feature.GIBDD_DYNAMICS| ProviderPaymentActivity| |  |
| https://online.alfabank.ru/multistep_invoice
alfabank://multistep_invoice| Внешний| Параметр - invoiceID| | | ProviderPaymentActivity| |  |
| https://online.alfabank.ru/fns
alfabank://fns| Внешний| | | Feature.GOS_PAYMENTS| ProviderPaymentActivity| |  |
| https://sberbank.ru/qr/| Внешний| | | | ProviderPaymentActivity| |  |
| https://online.alfabank.ru/push_settings
alfabank://push_settings| Внешний| | | Feature.PUSH_SETTINGS| PushSettingsActivity| |  |
| https://online.alfabank.ru/qr_auth
alfabank://qr_auth| Внешний| | | Feature.ALFA_CLICK_QR_AUTH| QrScannerActivity| |  |
| bank100000000008://sub.nspk.ru (path может быть любой, а может и не быть вообще)| Внешний| | | | QrNspkActivity| |  |
| bank100000000008://qr.nspk.ru (path может быть любой, а может и не быть вообще)| Внешний| | | | QrNspkActivity| |  |
| bank100000000008://sbpay (path может быть любой, а может и не быть вообще)| Внешний| | | | QrNspkActivity| |  |
| https://online.alfabank.ru/qr_payment
alfabank://qr_payment| Внешний| | | Feature.QR_PAYMENTS| QrScannerActivity| |  |
| https://online.alfabank.ru/quick_requests
alfabank://quick_requests| Внешний| | | Feature.QUICK_REQUEST| QuickRequestsRecipientSelectActivity| |  |
| https://online.alfabank.ru/credit_card_account_tariff
alfabank://credit_card_account_tariff| Внешний| Параметр - account_number| | Feature.CREDIT_RATES| RatesActivity| |  |
| https://online.alfabank.ru/card_tariff
alfabank://card_tariff| Внешний| Параметр - id| | Feature.CUSTOM_CARD_RATES_BUTTON| RatesActivity| |  |
| https://online.alfabank.ru/account_recharge
alfabank://account_recharge| Внешний| Параметр - currency
Параметр - minor_units
Параметр - amount
Параметр - account_number| | Feature.CREDIT_PAYMENT_INSUFFICIENT_FUNDS_RECHARGE| RechargeChooseActivity| |  |
| https://online.alfabank.ru/referral_details
alfabank://referral_details| Внешний| Параметр - categoryId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 2,
	- описание - id категории продуктов.
Параметр - productId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 2,
	- описание - id выбранного продукта.
Параметр - typeId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 5,
	- описание - id типа оффера.
Параметр - advTypeId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 6,
	- описание - id типа рекламного оффера.
Параметр - advCategoryId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 6,
	- описание - id категории рекламного оффера.| /referral_details?typeId=5&categoryId=2&productId=2
| Feature.REFERRAL, Feature.REFERRAL_MVI| MviReferralDetailsActivity, ReferralDetailsActivity| 11.28| Диплинк на экран с детальной информацией по продуктам в категории. При включенном ФТ REFERRAL_MVI +
открывается экран с детальной информацией на архитектуре MVI |
| https://online.alfabank.ru/referral_dynamic_details
alfabank://referral_dynamic_details| Внешний| Параметр - typeId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 2,
	- описание - id типа оффера.
Параметр - categoryId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 2,
	- описание - id категории продуктов.
Параметр - productId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 2,
	- описание - id выбранного продукта.| /referral_dynamic_details?typeId=2&categoryId=2&productId=2
| Feature.REFERRAL, Feature.REFERRAL_DYNAMIC_DETAILS| ReferralDynamicDetailsActivity| 11.55| Если включены ft Feature.REFERRAL и ft Feature.REFERRAL_DYNAMIC_DETAILS, и в диплинке +
присутствуют параметры typeId, categoryId и productId, то откроется экран детальной информации о продукте +
на динамополях. Если одно из условий не выполнено, то ничего не откроется |
| https://online.alfabank.ru/referral_showcase
alfabank://referral_showcase| Внешний| Параметр - typeId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 2,
	- описание - id типа оффера.
Параметр - advTypeId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 6,
	- описание - id типа рекламного оффера.
Параметр - advCategoryId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: 6,
	- описание - id категории рекламного оффера.| /referral_showcase
| Feature.REFERRAL, Feature.REFERRAL_MVI| MviReferralShowcaseActivity, ReferralShowcaseActivity| 11.28| Диплинк на экран-витрину реферальной программы. При включенном ФТ REFERRAL_MVI +
открывается экран-витрина реферальной программы на архитектуре MVI |
| https://online.alfabank.ru/referral_history
alfabank://referral_history| Внешний| | /referral_history
| Feature.REFERRAL, Feature.REFERRAL_HISTORY_WITH_FILTERS| ReferralHistoryActivity, ReferralHistoryWithFiltersActivity| 11.28| Если включен ft Feature.REFERRAL, откроется один из двух экранов истории рефералки: +
Если включен ft Feature.REFERRAL_HISTORY_WITH_FILTERS, то откроется экран ReferralHistoryWithFiltersActivity +
иначе откроется экран ReferralHistoryActivity. +
Если ft Feature.REFERRAL выключен, то ничего не откроется |
| https://online.alfabank.ru/credit_conditions
alfabank://credit_conditions| Внешний| Параметр - contract_number| | Feature.CREDIT_CONDITIONS| ReplenishActivity| |  |
| https://online.alfabank.ru/restaurants_and_lounges_compensations
alfabank://restaurants_and_lounges_compensations| Внешний| | | Feature.NON_FINANCIAL_RESTAURANTS_AND_LOUNGES| RestaurantsAndLoungesCompensationsActivity| |  |
| https://online.alfabank.ru/user_profile/bonuses/reverse_cashback
alfabank://user_profile/bonuses/reverse_cashback| Внешний| | | Feature.BOOMERANG_CARD_DETAILS_ENABLED| ReverseCashBackMainActivity| |  |
| https://online.alfabank.ru/user_profile/safeboxes
alfabank://user_profile/safeboxes| Внешний| | | Feature.SAFEBOX_DEPOSIT| SafeboxListActivity| |  |
| https://online.alfabank.ru/user_profile/safeboxes/safebox
alfabank://user_profile/safeboxes/safebox| Внешний| Параметр - id| | Feature.SAFEBOX_DEPOSIT| SafeboxDetailsActivity, SafeboxDetailsOldActivity| |  |
| https://online.alfabank.ru/salary_antislavery
alfabank://salary_antislavery| Внешний| | | Feature.SALARY_ANTISLAVERY| SalaryAntislaveryActivity| |  |
| https://online.alfabank.ru/sdui_screen
alfabank://sdui_screen| Внешний| Параметр - presentationType
Параметр - toolbarColor
Параметр - endpoint
Параметр - title
Параметр - subtitle| | | SDUIScreenActivity, SDUIScreenEmptyActivity| |  |
| https://online.alfabank.ru/user_profile/detail/code_word
alfabank://user_profile/detail/code_word| Внешний| | | Feature.USER_PROFILE_VIEW_SECRET_WORD| SecretWordActivity| |  |
| https://online.alfabank.ru/user_profile/code_word
alfabank://user_profile/code_word| Внешний| | | Feature.USER_PROFILE_VIEW_SECRET_WORD| SecretWordActivity| |  |
| https://online.alfabank.ru/user_profile/detail/code_word_change_request
alfabank://user_profile/detail/code_word_change_request| Внешний| | | Feature.USER_PROFILE_VIEW_SECRET_WORD| SecretWordClaimActivity| |  |
| https://online.alfabank.ru/user_profile/self_employed
alfabank://user_profile/self_employed| Внешний| | | Feature.SELF_EMPLOYED_REGISTRATION, Feature.SELF_EMPLOYED_INCOME_HISTORY, Feature.SELF_EMPLOYED_REGISTER_INCOME_UNLIMITED, Feature.SELF_EMPLOYED_INVOICES, Feature.STATEMENT_OPERATION_DETAILS_CREATE_BILL| SelfEmployedActivity| |  |
| https://online.alfabank.ru/self_employed_registration
alfabank://self_employed_registration| Внешний| | | Feature.SELF_EMPLOYED_REGISTRATION| RegistrationActivity| |  |
| https://online.alfabank.ru/user_profile/benefits_details/history
alfabank://user_profile/benefits_details/history| Внешний| Параметр - calculationDate| | Feature.PACKAGE_BENEFITS| FreeServiceHistoryActivity| |  |
| https://online.alfabank.ru/premium_travel_insurance
alfabank://premium_travel_insurance| Внешний| Параметр - title
Параметр - detailsEndpoint
Параметр - backgroundUrl| | Feature.BONUS_AVAILABLE| BonusDetailsActivity| |  |
| https://online.alfabank.ru/user_profile/benefits_details
alfabank://user_profile/benefits_details| Внешний| | | Feature.PACKAGE_BENEFITS| FreeServiceTermsActivity| |  |
| https://online.alfabank.ru/user_profile/benefits_discount
alfabank://user_profile/benefits_discount| Внешний| | | Feature.PACKAGE_BENEFITS| FreeServiceInfoActivity| |  |
| https://online.alfabank.ru/user_profile/bonuses/concierge
alfabank://user_profile/bonuses/concierge| Внешний| | | Feature.BONUS_AVAILABLE| BonusDetailsActivity| |  |
| https://online.alfabank.ru/balance_transfer
alfabank://balance_transfer| Внешний| | | Feature.BALANCE_TRANSFERS| BalanceTransferOfferActivity| |  |
| https://online.alfabank.ru/bonuses
alfabank://bonuses| Внешний| | | | ServiceInfoActivity, ServiceInfoRedesignActivity| |  |
| /incomplete_operations/sign_operation_at_branch_history| Внутренний| | | Feature.SIGN_ONLINE_APPROVED_OPERATION_HISTORY| SignedDocumentsActivity| |  |
| https://online.alfabank.ru/dynamic_fields_screen
alfabank://dynamic_fields_screen| Внешний| Параметр - endpoint
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: v1/debit-card-order/onboarding/third-party?stepId=1%26reference=H540903230000044,
	- описание - 
                Ручка, которая будет отдавать DynamicLongreadModel (диполя).
                Используется только в simple_dynamic_longread.
                Внедрен в версии 11.54
            .
Параметр - category
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - 
                Категория для аналитики экрана.
                Используется только в simple_dynamic_longread.
                Внедрен в версии 11.65
            .
Параметр - screenName
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - 
                Название экрана для аналитики экрана.
                Используется только в simple_dynamic_longread.
                Внедрен в версии 11.65
            .
Параметр - pageId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - 
                Id для загрузки конкретной страницы фичи.
                Конкретная реализация может иметь собственную обработку этого параметра.
                Внедрен в версии 11.65
            .
Параметр - isReloadDataWhenDisplay
	- не опцианальное,
	- дефолтное значение - false,
	- описание - 
                Перезагрузка данных в колбеке onResume.
                Используется только в simple_dynamic_longread.
                Внедрен в версии 11.68
            .
Параметр - useDynamicNavIcon
	- не опцианальное,
	- дефолтное значение - false,
	- описание - 
                Активация возможности передачи кастомных иконок в навбар.
                Конкретная реализация может отключить необходимость передачи этого флага.
                Внедрен в версии 12.05
            .| https://online.alfabank.ru/dynamic_fields_screen?useDynamicNavIcon=true&endpoint=v1/debit-card-order/onboarding/third-party?stepId=1%26reference=H540903230000044
alfabank:///dynamic_fields_screen?useDynamicNavIcon=true&endpoint=v1/debit-card-order/onboarding/third-party?stepId=1%26reference=H540903230000044
| Feature.DYNAMIC_FIELDS_SCREEN_V2, Feature.DYNAMIC_FIELDS_SCREEN| DynamicFieldsActivity, SimpleDynamicLongreadActivity| 11.54| Экран для загрузки и отображения динамополей с аналитикой, отображением ошибок и прочей общей логикой.

Если включен ft Feature.DYNAMIC_FIELDS_SCREEN_V2, откроется новый экран SimpleDynamicLongreadActivity,
Если включен ft Feature.DYNAMIC_FIELDS_SCREEN, откроется экран DynamicFieldsActivity, иначе ничего не открывается |
| /social_treasury_uzesia| Внутренний| Параметр - status
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: SUCCESSFUL, PROCESSING, FAILED,
	- описание - Статус подтверждённости УЗ на портале ЕСИА..| /social_treasury_uzesia?status=SUCCESSFUL
/social_treasury_uzesia?status=PROCESSING
/social_treasury_uzesia?status=FAILED
| Feature.SOCIAL_TREASURY| SocialTreasuryResultActivity| 12.04| Диплинк необходим для отправки статуса на мидл и получения дальнейшего диплинка.\n +
Если status == SUCCESSFUL, получим диплинк на возобновление многошага, иначе - на главный экран.\n +
Если включен FT SOCIAL_TREASURY, откроется экран SocialTreasuryResultActivity. |
| /social_treasury_final| Внутренний| | /social_treasury_final
| Feature.SOCIAL_TREASURY| SocialTreasuryResultActivity| 12.04| При включённом FT SOCIAL_TREASURY откроется экран SocialTreasuryResultActivity. |
| https://online.alfabank.ru/social_treasury
alfabank://social_treasury| Внешний| Параметр - transactionId
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - ID транзакции многошага. Используется только для внутренней навигации,  +
                    диплинк присылает мидл после выхода из многошага по флоу и необходимости вернуться..| /social_treasury
/social_treasury?transactionId=123
| Feature.SOCIAL_TREASURY| DynamicMultistepActivity| 12.04| Точка входа в фичу. Используется в смс рассылках и в баннере на главном экране.\n +
Также используется во внутренней навигации для возобновления многошага.\n +
При включенном FT SOCIAL_TREASURY откроется экран DynamicMultistepActivity. |
| /user_profile/social_treasury| Внутренний| | /user_profile/social_treasury
| Feature.SOCIAL_TREASURY| DynamicMultistepActivity| 12.04| Точка входа в фичу, вход с экрана профиля.\n +
При включенном FT SOCIAL_TREASURY откроется экран DynamicMultistepActivity. |
| /account_information/social_treasury| Внутренний| | /account_information/social_treasury
| Feature.SOCIAL_TREASURY| DynamicMultistepActivity| 12.04| Точка входа в фичу, вход с экрана счёта.\n +
При включенном FT SOCIAL_TREASURY откроется экран DynamicMultistepActivity. |
| https://online.alfabank.ru/marketplace_offers
alfabank://marketplace_offers| Внешний| | | Feature.NEW_MARKETPLACE| SpecialForYouActivity| |  |
| https://online.alfabank.ru/state_services_crossroad
alfabank://state_services_crossroad| Внешний| | | Feature.STATE_SERVICES_CROSSROAD| StateServicesCrossroadActivity| |  |
| https://online.alfabank.ru/statement
alfabank://statement| Внешний| | | Feature.OPERATIONS_HISTORY, Feature.REDESIGN, Feature.BOTTOM_NAVIGATION, Feature.BOTTOM_NAVIGATION_FOR_THIRD_PARTY_CLIENT| OperationsHistoryActivity, StatementActivity, intent
            .putExtra(EXTRA_NAVIGATION_MENU_SCREEN, mainScreen)
            .putExtra(EXTRA_DEFAULT_CHAT_MESSAGE, defaultMessage)
            .putExtra(EXTRA_SHOULD_REFRESH, shouldRefresh)
            .addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP or Intent.FLAG_ACTIVITY_SINGLE_TOP)| |  |
| /invoice_subscriptions_edit| Внутренний| Параметр - subscriptionId
Параметр - paySys| | Feature.INVOICE_DASHBOARD_V2| | |  |
| /invoice_subscriptions| Внутренний| Параметр - providerGroup
Параметр - providerId| | Feature.INVOICE_DASHBOARD_V2| SubscriptionsControlActivity| |  |
| https://online.alfabank.ru/payments_dashboard/categories
alfabank://payments_dashboard/categories| Внешний| Параметр - category
Параметр - source
Параметр - subscriptionId| | Feature.INVOICE_DASHBOARD_V2| CategoryActivity| |  |
| https://online.alfabank.ru/autosubscription
alfabank://autosubscription| Внешний| | | Feature.AM_BILLS_FOR_PAYMENTS| InvoicesActivity, SubscriptionsInvoicesActivity| |  |
| https://online.alfabank.ru/subscriptions_management
alfabank://subscriptions_management| Внешний| | | Feature.SUBSCRIPTIONS_MANAGEMENT| SubscriptionsManagementMainActivity| |  |
| /info_channels/support_call| Внутренний| | info_channels/support_call?lastDestinationOnly=false
| Feature.CALL_SUPPORT| SupportCallActivity| 12.04| Если включен ФТ CALL_SUPPORT, открывает экран ip звонка с поддержкой бэкстэка на экран каналов |
| https://online.alfabank.ru/support_call
alfabank://support_call| Внешний| | | Feature.CALL_SUPPORT| SupportCallActivity| |  |
| https://online.alfabank.ru/communication_source
alfabank://communication_source| Внешний| Параметр - id| | Feature.INFO_CHANNELS| ChannelActivity| |  |
| https://online.alfabank.ru/user_profile/whats_new_channel
alfabank://user_profile/whats_new_channel| Внешний| | | Feature.WHATS_NEW_CHANNEL| ChannelActivity| |  |
| /investments/documents/dynamic-list| Внутренний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - идентификатор актива.
Параметр - type
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - тип актива.| /investments/pif?id=BVAAD2F&type=MUTUAL
| Feature.INVESTMENTS_PIFS_PURCHASE_REDESIGN| SifDocumentsHostActivity| 11.44| Диплинк на документ информации об активе |
| https://online.alfabank.ru/investments/recommendations
alfabank://investments/recommendations| Внешний| | | Feature.INVESTMENTS_RECOMMENDATIONS| SifRecommendationHostActivity| |  |
| /investments/default_recommendation| Внутренний| | | Feature.INVESTMENTS_RECOMMENDATIONS| SifRecommendationHostActivity| |  |
| https://online.alfabank.ru/investments/profile_screen
alfabank://investments/profile_screen| Внешний| Параметр - deeplink
Параметр - deeplinkType| | Feature.INVESTMENTS_RECOMMENDATIONS| SifRecommendationHostActivity| |  |
| /investments/pif/repay| Внутренний| Параметр - id| | Feature.INVESTMENTS_PIFS_SELL_REDESIGN| PifsSellActivity, SifInvestmentsPifsHostActivity| |  |
| /investments/pif/buy| Внутренний| Параметр - id
Параметр - number
Параметр - date
Параметр - id
Параметр - title
Параметр - portfolio| | Feature.INVESTMENTS_PIFS_PURCHASE_REDESIGN, Feature.INVESTMENTS_PIFS_PURCHASE_REDESIGN| PifsOrderPurchaseActivity, PifsPaymentActivity, SifInvestmentsPifsHostActivity| |  |
| /investments/pif/exchange| Внутренний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - идентификатор ПИФа.| /investments/pif/exchange?id=BVAAD2F
| | PifsExchangeCatalogueActivity| 11.44| Диплинк на экран обмена ПИФа |
| https://online.alfabank.ru/investments/strategy
alfabank://investments/strategy| Внешний| Параметр - id| | | SifProductCardHostActivity| |  |
| https://online.alfabank.ru/investments/pif
alfabank://investments/pif| Внешний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - идентификатор ПИФа.| /investments/pif/exchange?id=BVAAD2F
| | SifProductCardHostActivity| 11.44| Диплинк на карточку ПИФа. Внедрен в 2019г. в модуле investments_pifs  +
Перенесен в новый модуль с версии 11.44 +
откроется новый экран SifProductCardHostActivity, |
| /investments/strategy/purchase| Внутренний| Параметр - strategyID| | | SifInvestmentsTrustsHostActivity| |  |
| /investments/strategy/opening| Внутренний| Параметр - status
Параметр - strategyID
Параметр - currency| | | SifInvestmentsTrustsHostActivity| |  |
| https://online.alfabank.ru/card_progress_cashback
alfabank://card_progress_cashback| Внешний| Параметр - id
Параметр - title| | Feature.CARD_DETAILS_CASHBACK_CONDITIONS| CashBackConditionsActivity| |  |
| https://online.alfabank.ru/user_profile/interest_on_balance
alfabank://user_profile/interest_on_balance| Внешний| | | Feature.USER_PROFILE_INTEREST_ON_BALANCE| InterestOnBalanceActivity| |  |
| https://online.alfabank.ru/card_progress_conditions
alfabank://card_progress_conditions| Внешний| Параметр - id
Параметр - title
Параметр - isCardTariffAvailable| | Feature.CARD_DETAILS_TARIFF_CONDITIONS| TariffConditionsActivity| |  |
| https://online.alfabank.ru/view_autopayments
alfabank://view_autopayments| Внешний| | | Feature.TEMPLATES_REDESIGN| TemplatesActivity| |  |
| https://online.alfabank.ru/templates
alfabank://templates| Внешний| | | | MyPaymentsActivity, TemplatesActivity| |  |
| https://online.alfabank.ru/my_payments
alfabank://my_payments| Внешний| | | | MyPaymentsActivity, TemplatesActivity| |  |
| https://online.alfabank.ru/template_creation
alfabank://template_creation| Внешний| Параметр - reference| | | CreateTemplateActivity| |  |
| /template_details| Внутренний| Параметр - templateId
Параметр - listType
Параметр - title
Параметр - myPaymentsType
Параметр - route| | Feature.AM_OPEN_TEMPLATE_DETAILS_SCREEN| TemplateDetailsActivity| |  |
| https://online.alfabank.ru/user_profile/bonuses/transfers
alfabank://user_profile/bonuses/transfers| Внешний| | | Feature.BONUS_AVAILABLE| TransfersActivity| |  |
| https://online.alfabank.ru/taxi_compensations
alfabank://taxi_compensations| Внешний| | | Feature.NON_FINANCIAL_TAXI| TransfersRefundActivity| |  |
| /user_profile_travel_insurance| Внутренний| Параметр - id
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - id страхового полиса.| /user_profile_travel_insurance?id=03432%2F118%2F13030325
| Feature.TRAVEL_INSURANCE| TravelInsuranceDetailsActivity| 11.26| Диплинк для перехода на экран информации о полисе |
| https://online.alfabank.ru/travel_insurance
alfabank://travel_insurance| Внешний| | /travel_insurance
| Feature.TRAVEL_INSURANCE| TravelInsuranceAcquireActivity| 11.26| Диплинк для перехода на экран оформления полиса страхования в путешествии |
| https://online.alfabank.ru/trusted_persons
alfabank://trusted_persons| Внешний| | | Feature.TRUSTED_PERSONS| TrustedPersonsActivity| |  |
| https://online.alfabank.ru/operations_quick_money_request
alfabank://operations_quick_money_request| Внешний| | | Feature.QUICK_REQUEST| UnapprovedOperationListActivity, UnapprovedOperationsWithSignOnlineActivity| |  |
| https://online.alfabank.ru/incomplete_operations
alfabank://incomplete_operations| Внешний| | | | UnapprovedOperationListActivity, UnapprovedOperationsWithSignOnlineActivity| |  |
| /rate_app| Внутренний| | | | Uri.parse(intentUrl)| |  |
| https://online.alfabank.ru/update_app
alfabank://update_app| Внешний| | | | UpdateAppActivity| |  |
| https://online.alfabank.ru/user_profile/detail/embossed_name
alfabank://user_profile/detail/embossed_name| Внешний| | | Feature.USER_EMBOSSED_NAME_CHANGE| ChangeEmbossedNameActivity| |  |
| https://online.alfabank.ru/user_profile/embossed_name
alfabank://user_profile/embossed_name| Внешний| | | Feature.USER_EMBOSSED_NAME_CHANGE| ChangeEmbossedNameActivity| |  |
| https://online.alfabank.ru/user_profile/user_policies
alfabank://user_profile/user_policies| Внешний| | | Feature.USER_POLICIES| UserPoliciesActivity| |  |
| /user_profile/change_user_avatar| Внутренний| Параметр - canDelete
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: true, false,
	- описание - Возможность удаления аватара.| /profile/user_avatar_change?canDelete=true
| Feature.USER_PROFILE_REDESIGN, Feature.CHANGE_USER_AVATAR| UserProfileActivity| 12.02| Если включены ФТ USER_PROFILE_REDESIGN и ФТ CHANGE_USER_AVATAR, открывает BottomSheet на новом  +
экране профиля с выбором действий для аватара, иначе ничего не происходит |
| https://online.alfabank.ru/user_profile
alfabank://user_profile| Внешний| | | Feature.USER_PROFILE_REDESIGN, Feature.WIDGET_USER_PROFILE| OldUserProfileWidgetActivity, UserProfileActivity| 12.02| Если включен ФТ USER_PROFILE_REDESIGN, открывает новый экран профиля, иначе открывает старый экран профиля, если
включен ФТ WIDGET_USER_PROFILE |
| https://online.alfabank.ru/user_profile/statements_order
alfabank://user_profile/statements_order| Внешний| | | Feature.STATEMENT_ORDER_WEBVIEW| WebFeatureActivity| |  |
| https://online.alfabank.ru/branch_vip_appointment_registration
alfabank://branch_vip_appointment_registration| Внешний| | | Feature.VIP_APPOINTMENT_ENTRYPOINTS| VipVisitRegistrationActivity| |  |
| https://online.alfabank.ru/branch_vip_appointment
alfabank://branch_vip_appointment| Внешний| Параметр - id| | Feature.VIP_APPOINTMENT_ENTRYPOINTS| VipFullVisitInfoActivity| |  |
| https://online.alfabank.ru/branch_appointment_registration
alfabank://branch_appointment_registration| Внешний| | | Feature.APPOINTMENT_ENTRYPOINTS| ChooseCategoryActivity| |  |
| https://online.alfabank.ru/branch_appointment
alfabank://branch_appointment| Внешний| Параметр - id| | Feature.APPOINTMENT_ENTRYPOINTS| FullVisitInfoActivity| |  |
| https://online.alfabank.ru/feedback
alfabank://feedback| Внешний| Параметр - id
Параметр - type| | Feature.DEEPLINK_CUSTOMER_FEEDBACK| VocSurveyActivity| |  |
| https://online.alfabank.ru/voice_assistant
alfabank://voice_assistant| Внешний| | | Feature.VOICE_ASSISTANT| VoiceAssistantActivity| |  |
| https://online.alfabank.ru/user_profile/voyage_details
alfabank://user_profile/voyage_details| Внешний| | | Feature.VOYAGE_DETAILS| VoyageDetailsActivity| |  |
| https://online.alfabank.ru/forex
alfabank://forex| Внешний| | | Feature.FOREX| WebFeatureActivity| |  |
| https://online.alfabank.ru/budget_payment
alfabank://budget_payment| Внешний| | | Feature.TAX_PAYMENT| WebFeatureActivity| |  |
| /loyalty_wheel_of_fortune| Внутренний| Параметр - targetDate
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - дата текущего предложения.| /loyalty_wheel_of_fortune?targetDate=01-01-2020
| | WheelOfFortuneActivity| 11.54| Открывает новый экран WheelOfFortuneActivity,
при отсутствии какого либо параметра в uri, ничего не откроется |
| /loyalty_wheel_of_fortune_final| Внутренний| Параметр - targetDate
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- описание - дата текущего предложения.| /loyalty_wheel_of_fortune_final?targetDate=01-01-2020
| | WheelOfFortuneFinalActivity| 11.54| Открывает новый экран WheelOfFortuneFinalActivity,
при отсутствии какого либо параметра в uri, ничего не откроется |
| https://online.alfabank.ru/where_to_begin
alfabank://where_to_begin| Внешний| | | Feature.WHERE_TO_BEGIN| WhereToBeginActivity| |  |
| https://online.alfabank.ru/user_profile/caller_id
alfabank://user_profile/caller_id| Внешний| | | Feature.KASPERSKY_WHO_CALLS| OnboardingWhoCallsActivity| |  |
| https://online.alfabank.ru/user_profile/settings/caller_id
alfabank://user_profile/settings/caller_id| Внешний| | | Feature.KASPERSKY_WHO_CALLS| OnboardingWhoCallsActivity| |  |
| /widget_screen| Внутренний| Параметр - endpoint
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: /%2Fwidget-management%2Fscreens%2FmyBusiness,
	- описание - Эндпоинт для загрузки виджетов.
Параметр - screenName
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: myBusiness,
	- описание - Имя экрана, используется для аналитики.
Параметр - style
	- не опцианальное,
	- дефолтное значение - white,
	- примеры: gray, white,
	- описание - Стиль экрана(цвет фона).
Параметр - screenTitle
	- не опцианальное,
	- дефолтное значение - пустая строка,
	- примеры: Мой бизнес,
	- описание - Заголовок в тулбаре.| /widget_screen?endpoint=v1%2Fwidget-management%2Fscreens%2FmyBusiness&style=white&screenTitle=Мой%20бизнес
| Feature.WIDGET_SCREEN| SimpleWidgetsActivity| 12.02| Открывает виджетный экран |
| https://online.alfabank.ru/widget_settings
alfabank://widget_settings| Внешний| | | | WidgetSettingsActivity, WidgetToggleActivity| |  |
| https://online.alfabank.ru/user_profile/bonuses/yandex_plus
alfabank://user_profile/bonuses/yandex_plus| Внешний| | | Feature.YANDEX_PLUS_CASHBACK| YandexPlusCashBackActivity| |  |

Если в path отсутсвует https://online.alfabank.ru - то это диплинк для внутреннего использования. Внешний диплинк - диплинк по которому можно попасть в АльфаМобайл из сторонних программ, например кликнули по ссылке в СМС, внутренние диплинки используются только внутри АльфаМобайл, например для навигации в виджетах