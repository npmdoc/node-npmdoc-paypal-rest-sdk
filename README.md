# api documentation for  [paypal-rest-sdk (v1.7.1)](https://github.com/paypal/PayPal-node-SDK)  [![npm package](https://img.shields.io/npm/v/npmdoc-paypal-rest-sdk.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-paypal-rest-sdk) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-paypal-rest-sdk.svg)](https://travis-ci.org/npmdoc/node-npmdoc-paypal-rest-sdk)
#### SDK for PayPal REST APIs

[![NPM](https://nodei.co/npm/paypal-rest-sdk.png?downloads=true)](https://www.npmjs.com/package/paypal-rest-sdk)

[![apidoc](https://npmdoc.github.io/node-npmdoc-paypal-rest-sdk/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-paypal-rest-sdk_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-paypal-rest-sdk/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-paypal-rest-sdk/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-paypal-rest-sdk/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "PayPal",
        "email": "DL-PP-NODEJS-SDK@paypal.com",
        "url": "https://developer.paypal.com/"
    },
    "bugs": {
        "url": "https://github.com/paypal/PayPal-node-SDK/issues",
        "email": "DL-PP-NODEJS-SDK@paypal.com"
    },
    "config": {
        "blanket": {
            "pattern": "lib",
            "data-cover-never": "node_modules"
        }
    },
    "dependencies": {
        "buffer-crc32": "^0.2.3",
        "semver": "^5.0.3",
        "uuid": "^2.0.1"
    },
    "description": "SDK for PayPal REST APIs",
    "devDependencies": {
        "blanket": "~1.1.5",
        "chai": "~1.9.1",
        "coveralls": "~2.0.16",
        "grunt": "~0.4.1",
        "grunt-contrib-jshint": "~0.3.0",
        "grunt-jsdoc": "^0.5.8",
        "grunt-simple-mocha": "~0.4.0",
        "ink-docstrap": "^0.5.2",
        "jsdoc": "^3.3.0-beta1",
        "mocha": "~1.18.2",
        "mocha-lcov-reporter": "0.0.1",
        "nock": "0.36.2"
    },
    "directories": {},
    "dist": {
        "shasum": "1d73885cc775c38fb9b165d060a6c62138f400bd",
        "tarball": "https://registry.npmjs.org/paypal-rest-sdk/-/paypal-rest-sdk-1.7.1.tgz"
    },
    "engines": {
        "node": ">= v0.6.0"
    },
    "gitHead": "28c30c723268ac395ee06ceecf58013be6dbd5f3",
    "homepage": "https://github.com/paypal/PayPal-node-SDK",
    "keywords": [
        "paypal",
        "rest",
        "api",
        "sdk"
    ],
    "license": "SEE LICENSE IN https://github.com/paypal/PayPal-node-SDK/blob/master/LICENSE",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "paypal",
            "email": "DL-PP-Platform-NodeJs-SDK@ebay.com"
        }
    ],
    "man": [
        "README.md"
    ],
    "name": "paypal-rest-sdk",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/paypal/PayPal-node-SDK.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "version": "1.7.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module paypal-rest-sdk](#apidoc.module.paypal-rest-sdk)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.</span>configure (options)](#apidoc.element.paypal-rest-sdk.configure)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.</span>generateToken (config, cb)](#apidoc.element.paypal-rest-sdk.generateToken)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.</span>generate_token (config, cb)](#apidoc.element.paypal-rest-sdk.generate_token)
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>api
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>authorization
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>billingAgreement
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>billingPlan
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>billing_agreement
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>billing_plan
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>capture
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>client
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>configuration
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>creditCard
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>credit_card
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>generate
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>invoice
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>invoiceTemplate
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>notification
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>openIdConnect
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>openIdConnect.tokeninfo
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>openIdConnect.userinfo
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>openid_connect
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>openid_connect.tokeninfo
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>openid_connect.userinfo
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>order
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>payment
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>payout
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>payoutItem
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>refund
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>sale
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>utils
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.</span>webProfile
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.</span>version

#### [module paypal-rest-sdk.api](#apidoc.module.paypal-rest-sdk.api)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.api.</span>configure (options)](#apidoc.element.paypal-rest-sdk.api.configure)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.api.</span>executeHttp (http_method, path, data, http_options, cb)](#apidoc.element.paypal-rest-sdk.api.executeHttp)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.api.</span>generateToken (config, cb)](#apidoc.element.paypal-rest-sdk.api.generateToken)

#### [module paypal-rest-sdk.authorization](#apidoc.module.paypal-rest-sdk.authorization)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>capture (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.capture)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>reauthorize (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.reauthorize)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>void (id, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.void)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>baseURL

#### [module paypal-rest-sdk.billingAgreement](#apidoc.module.paypal-rest-sdk.billingAgreement)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>billBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.billBalance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>bill_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.bill_balance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>cancel (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.cancel)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>execute (token, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.execute)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>reactivate (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.reactivate)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>searchTransactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.searchTransactions)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>search_transactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.search_transactions)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>setBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.setBalance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>set_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.set_balance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>suspend (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.suspend)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>baseURL

#### [module paypal-rest-sdk.billingPlan](#apidoc.module.paypal-rest-sdk.billingPlan)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>activate (id, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.activate)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>baseURL

#### [module paypal-rest-sdk.billing_agreement](#apidoc.module.paypal-rest-sdk.billing_agreement)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>billBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.billBalance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>bill_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.bill_balance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>cancel (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.cancel)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>execute (token, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.execute)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>reactivate (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.reactivate)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>searchTransactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.searchTransactions)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>search_transactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.search_transactions)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>setBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.setBalance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>set_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.set_balance)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>suspend (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.suspend)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>baseURL

#### [module paypal-rest-sdk.billing_plan](#apidoc.module.paypal-rest-sdk.billing_plan)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>activate (id, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.activate)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>baseURL

#### [module paypal-rest-sdk.capture](#apidoc.module.paypal-rest-sdk.capture)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.capture.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.capture.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.capture.</span>refund (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.capture.refund)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.capture.</span>baseURL

#### [module paypal-rest-sdk.client](#apidoc.module.paypal-rest-sdk.client)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.client.</span>invoke (http_method, path, data, http_options_param, cb)](#apidoc.element.paypal-rest-sdk.client.invoke)

#### [module paypal-rest-sdk.creditCard](#apidoc.module.paypal-rest-sdk.creditCard)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.del)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.delete)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>baseURL

#### [module paypal-rest-sdk.credit_card](#apidoc.module.paypal-rest-sdk.credit_card)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.del)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.delete)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>baseURL

#### [module paypal-rest-sdk.generate](#apidoc.module.paypal-rest-sdk.generate)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.generate.</span>mixin (destObject, operations)](#apidoc.element.paypal-rest-sdk.generate.mixin)

#### [module paypal-rest-sdk.invoice](#apidoc.module.paypal-rest-sdk.invoice)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>cancel (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.cancel)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.del)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.delete)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>deleteExternalPayment (invoiceId, transactionId, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.deleteExternalPayment)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>deleteExternalRefund (invoiceId, transactionId, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.deleteExternalRefund)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>generateNumber (config, cb)](#apidoc.element.paypal-rest-sdk.invoice.generateNumber)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>qrCode (id, height, width, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.qrCode)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>recordPayment (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.recordPayment)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>recordRefund (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.recordRefund)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>remind (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.remind)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>search (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.search)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>send (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.send)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>baseURL

#### [module paypal-rest-sdk.invoiceTemplate](#apidoc.module.paypal-rest-sdk.invoiceTemplate)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.delete)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>baseURL

#### [module paypal-rest-sdk.openIdConnect](#apidoc.module.paypal-rest-sdk.openIdConnect)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>authorizeUrl (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.authorizeUrl)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>authorize_url (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.authorize_url)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>logoutUrl (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.logoutUrl)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>logout_url (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.logout_url)
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>tokeninfo
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>userinfo

#### [module paypal-rest-sdk.openIdConnect.tokeninfo](#apidoc.module.paypal-rest-sdk.openIdConnect.tokeninfo)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.tokeninfo.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.openIdConnect.tokeninfo.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.tokeninfo.</span>refresh (data, config, cb)](#apidoc.element.paypal-rest-sdk.openIdConnect.tokeninfo.refresh)

#### [module paypal-rest-sdk.openIdConnect.userinfo](#apidoc.module.paypal-rest-sdk.openIdConnect.userinfo)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.userinfo.</span>get (data, config, cb)](#apidoc.element.paypal-rest-sdk.openIdConnect.userinfo.get)

#### [module paypal-rest-sdk.openid_connect](#apidoc.module.paypal-rest-sdk.openid_connect)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>authorizeUrl (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.authorizeUrl)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>authorize_url (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.authorize_url)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>logoutUrl (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.logoutUrl)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>logout_url (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.logout_url)
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>tokeninfo
1.  object <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>userinfo

#### [module paypal-rest-sdk.openid_connect.tokeninfo](#apidoc.module.paypal-rest-sdk.openid_connect.tokeninfo)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.tokeninfo.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.openid_connect.tokeninfo.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.tokeninfo.</span>refresh (data, config, cb)](#apidoc.element.paypal-rest-sdk.openid_connect.tokeninfo.refresh)

#### [module paypal-rest-sdk.openid_connect.userinfo](#apidoc.module.paypal-rest-sdk.openid_connect.userinfo)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.userinfo.</span>get (data, config, cb)](#apidoc.element.paypal-rest-sdk.openid_connect.userinfo.get)

#### [module paypal-rest-sdk.order](#apidoc.module.paypal-rest-sdk.order)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>authorize (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.order.authorize)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>capture (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.order.capture)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.order.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>void (id, config, cb)](#apidoc.element.paypal-rest-sdk.order.void)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>baseURL

#### [module paypal-rest-sdk.payment](#apidoc.module.paypal-rest-sdk.payment)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>execute (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.execute)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.payment.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>baseURL

#### [module paypal-rest-sdk.payout](#apidoc.module.paypal-rest-sdk.payout)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payout.</span>create (data, sync_mode, config, cb)](#apidoc.element.paypal-rest-sdk.payout.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payout.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.payout.get)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.payout.</span>baseURL

#### [module paypal-rest-sdk.payoutItem](#apidoc.module.paypal-rest-sdk.payoutItem)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payoutItem.</span>cancel (id, config, cb)](#apidoc.element.paypal-rest-sdk.payoutItem.cancel)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.payoutItem.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.payoutItem.get)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.payoutItem.</span>baseURL

#### [module paypal-rest-sdk.refund](#apidoc.module.paypal-rest-sdk.refund)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.refund.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.refund.get)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.refund.</span>baseURL

#### [module paypal-rest-sdk.sale](#apidoc.module.paypal-rest-sdk.sale)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.sale.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.sale.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.sale.</span>refund (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.sale.refund)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.sale.</span>baseURL

#### [module paypal-rest-sdk.utils](#apidoc.module.paypal-rest-sdk.utils)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>checkExpiredToken (token_hash)](#apidoc.element.paypal-rest-sdk.utils.checkExpiredToken)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>getDefaultApiEndpoint (mode)](#apidoc.element.paypal-rest-sdk.utils.getDefaultApiEndpoint)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>getDefaultEndpoint (mode)](#apidoc.element.paypal-rest-sdk.utils.getDefaultEndpoint)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>merge (obj1, obj2, appendOnly)](#apidoc.element.paypal-rest-sdk.utils.merge)

#### [module paypal-rest-sdk.webProfile](#apidoc.module.paypal-rest-sdk.webProfile)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.create)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.del)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.delete)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.get)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.list)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>replace (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.replace)
1.  [function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.update)
1.  string <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>baseURL



# <a name="apidoc.module.paypal-rest-sdk"></a>[module paypal-rest-sdk](#apidoc.module.paypal-rest-sdk)

#### <a name="apidoc.element.paypal-rest-sdk.configure"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.</span>configure (options)](#apidoc.element.paypal-rest-sdk.configure)
- description and source-code
```javascript
function configure(options) {
    api.configure(options);
}
```
- example usage
```shell
...

  '''js
  var paypal = require('paypal-rest-sdk');
  '''
* Create config options, with parameters (mode, client_id, secret).

  '''js
  paypal.configure({
    'mode': 'sandbox', //sandbox or live
    'client_id': 'EBWKjlELKMYqRNQ6sYvFo64FtaRLRR5BdHEESmha49TM',
    'client_secret': 'EO422dn3gQLgDbuwqTjzrFgFtaRLRR5BdHEESmha49TM'
  });
  '''
* For multiple configuration support, have a look at the [sample](/samples/configuration/multiple_config.js)
* Invoke the rest api (eg: store a credit card) with required parameters (eg: data, config_options, callback).
...
```

#### <a name="apidoc.element.paypal-rest-sdk.generateToken"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.</span>generateToken (config, cb)](#apidoc.element.paypal-rest-sdk.generateToken)
- description and source-code
```javascript
function generateToken(config, cb) {
    api.generateToken(config, cb);
}
```
- example usage
```shell
...
module.exports = function () {

function configure(options) {
    api.configure(options);
}

function generateToken(config, cb) {
    api.generateToken(config, cb);
}

return {
    version: configuration.sdkVersion,
    configure: configure,
    configuration: configuration.default_options,
    generateToken: generateToken,
...
```

#### <a name="apidoc.element.paypal-rest-sdk.generate_token"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.</span>generate_token (config, cb)](#apidoc.element.paypal-rest-sdk.generate_token)
- description and source-code
```javascript
function generateToken(config, cb) {
    api.generateToken(config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.api"></a>[module paypal-rest-sdk.api](#apidoc.module.paypal-rest-sdk.api)

#### <a name="apidoc.element.paypal-rest-sdk.api.configure"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.api.</span>configure (options)](#apidoc.element.paypal-rest-sdk.api.configure)
- description and source-code
```javascript
function configure(options) {
    if (options !== undefined && typeof options === 'object') {
        configuration.default_options = utils.merge(configuration.default_options, options);
    }
}
```
- example usage
```shell
...

  '''js
  var paypal = require('paypal-rest-sdk');
  '''
* Create config options, with parameters (mode, client_id, secret).

  '''js
  paypal.configure({
    'mode': 'sandbox', //sandbox or live
    'client_id': 'EBWKjlELKMYqRNQ6sYvFo64FtaRLRR5BdHEESmha49TM',
    'client_secret': 'EO422dn3gQLgDbuwqTjzrFgFtaRLRR5BdHEESmha49TM'
  });
  '''
* For multiple configuration support, have a look at the [sample](/samples/configuration/multiple_config.js)
* Invoke the rest api (eg: store a credit card) with required parameters (eg: data, config_options, callback).
...
```

#### <a name="apidoc.element.paypal-rest-sdk.api.executeHttp"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.api.</span>executeHttp (http_method, path, data, http_options, cb)](#apidoc.element.paypal-rest-sdk.api.executeHttp)
- description and source-code
```javascript
function executeHttp(http_method, path, data, http_options, cb) {
    if (typeof http_options === "function") {
        cb = http_options;
        http_options = null;
    }
    if (!http_options) {
        http_options = configuration.default_options;
    } else {
        http_options = utils.merge(http_options, configuration.default_options, true);
    }

    //Get host endpoint using mode
    http_options.host = utils.getDefaultApiEndpoint(http_options.mode) || http_options.host;

    function retryInvoke() {
        client.invoke(http_method, path, data, http_options, cb);
    }

    // correlation-id is deprecated in favor of client-metadata-id
    if (http_options.client_metadata_id) {
        http_options.headers['Paypal-Client-Metadata-Id'] = http_options.client_metadata_id;
    }
    else if (http_options.correlation_id) {
        http_options.headers['Paypal-Client-Metadata-Id'] = http_options.correlation_id;
    }

    // If client_id exists with an unexpired token and a refresh token is not provided, reuse cached token
    if (http_options.client_id in token_persist && !utils.checkExpiredToken(token_persist[http_options.client_id]) && !http_options
.refresh_token) {
        http_options.headers.Authorization = "Bearer " + token_persist[http_options.client_id].access_token;
        client.invoke(http_method, path, data, http_options, function (error, response) {
            // Don't reprompt already authenticated user for login by updating Authorization header
            // if token expires
            if (error && error.httpStatusCode === 401 && http_options.client_id && http_options.headers.Authorization) {
                http_options.headers.Authorization = null;
                updateToken(http_options, cb, retryInvoke);
            } else {
                cb(error, response);
            }
        });
    } else {
        updateToken(http_options, cb, retryInvoke);
    }
}
```
- example usage
```shell
...
 * restFunctions Object containing the REST CRUD methods and paypal specific REST methods that
 * are shared between at least two of the REST endpoints, otherwise the function
 * will be defined within the resource definition itself
 * @type {Object}
 */
var restFunctions = {
create: function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
},
get: function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
},
list: function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
...
```

#### <a name="apidoc.element.paypal-rest-sdk.api.generateToken"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.api.</span>generateToken (config, cb)](#apidoc.element.paypal-rest-sdk.api.generateToken)
- description and source-code
```javascript
function generateToken(config, cb) {

    if (typeof config === "function") {
        cb = config;
        config = configuration.default_options;
    } else if (!config) {
        config = configuration.default_options;
    } else {
        config = utils.merge(config, configuration.default_options, true);
    }

    var payload = 'grant_type=client_credentials';
    if (config.authorization_code) {
        payload = 'grant_type=authorization_code&response_type=token&redirect_uri=urn:ietf:wg:oauth:2.0:oob&code=' + config.authorization_code
;
    } else if (config.refresh_token) {
        payload = 'grant_type=refresh_token&refresh_token=' + config.refresh_token;
    }

    var basicAuthString = 'Basic ' + new Buffer(config.client_id + ':' + config.client_secret).toString('base64');

    var http_options = {
        schema: config.schema || configuration.default_options.schema,
        host: utils.getDefaultApiEndpoint(config.mode) || config.host || configuration.default_options.host,
        port: config.port || configuration.default_options.port,
        headers: utils.merge({
            'Authorization': basicAuthString,
            'Accept': 'application/json',
            'Content-Type': 'application/x-www-form-urlencoded'
        }, configuration.default_options.headers, true)
    };

    client.invoke('POST', '/v1/oauth2/token', payload, http_options, function (err, res) {
        var token = null;
        if (res) {
            if (!config.authorization_code && !config.refresh_token) {
                var seconds = new Date().getTime() / 1000;
                token_persist[config.client_id] = res;
                token_persist[config.client_id].created_at = seconds;
            }

            if (!config.authorization_code) {
                token = res.token_type + ' ' + res.access_token;
            }
            else {
                token = res.refresh_token;
            }
        }
        cb(err, token);
    });
}
```
- example usage
```shell
...
module.exports = function () {

function configure(options) {
    api.configure(options);
}

function generateToken(config, cb) {
    api.generateToken(config, cb);
}

return {
    version: configuration.sdkVersion,
    configure: configure,
    configuration: configuration.default_options,
    generateToken: generateToken,
...
```



# <a name="apidoc.module.paypal-rest-sdk.authorization"></a>[module paypal-rest-sdk.authorization](#apidoc.module.paypal-rest-sdk.authorization)

#### <a name="apidoc.element.paypal-rest-sdk.authorization.capture"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>capture (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.capture)
- description and source-code
```javascript
function capture(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/capture', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.authorization.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.authorization.reauthorize"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>reauthorize (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.reauthorize)
- description and source-code
```javascript
function reauthorize(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/reauthorize', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.authorization.void"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.authorization.</span>void (id, config, cb)](#apidoc.element.paypal-rest-sdk.authorization.void)
- description and source-code
```javascript
function voidAuthorization(id, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/void', {}, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.billingAgreement"></a>[module paypal-rest-sdk.billingAgreement](#apidoc.module.paypal-rest-sdk.billingAgreement)

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.billBalance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>billBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.billBalance)
- description and source-code
```javascript
function billBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/bill-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.bill_balance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>bill_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.bill_balance)
- description and source-code
```javascript
function billBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/bill-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.cancel"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>cancel (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.cancel)
- description and source-code
```javascript
function cancel(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/cancel', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.execute"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>execute (token, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.execute)
- description and source-code
```javascript
function execute(token, data, config, cb) {
    //support case where neither data nor config is provided
    if (typeof data === "function" && arguments.length === 2) {
        cb = data;
        data = {};
    }
    api.executeHttp('POST', this.baseURL + token + '/agreement-execute', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.reactivate"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>reactivate (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.reactivate)
- description and source-code
```javascript
function reactivate(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/re-activate', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.searchTransactions"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>searchTransactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.searchTransactions)
- description and source-code
```javascript
function searchTransactions(id, start_date, end_date, config, cb) {
    var date_range = {
        "start_date": start_date,
        "end_date": end_date
    };
    api.executeHttp('GET', baseURL + id + '/transactions', date_range, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.search_transactions"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>search_transactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.search_transactions)
- description and source-code
```javascript
function searchTransactions(id, start_date, end_date, config, cb) {
    var date_range = {
        "start_date": start_date,
        "end_date": end_date
    };
    api.executeHttp('GET', baseURL + id + '/transactions', date_range, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.setBalance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>setBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.setBalance)
- description and source-code
```javascript
function setBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/set-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.set_balance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>set_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.set_balance)
- description and source-code
```javascript
function setBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/set-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.suspend"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>suspend (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.suspend)
- description and source-code
```javascript
function suspend(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/suspend', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingAgreement.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingAgreement.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingAgreement.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.billingPlan"></a>[module paypal-rest-sdk.billingPlan](#apidoc.module.paypal-rest-sdk.billingPlan)

#### <a name="apidoc.element.paypal-rest-sdk.billingPlan.activate"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>activate (id, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.activate)
- description and source-code
```javascript
function activate(id, config, cb) {
    var activate_attributes = [
        {
            "op": "replace",
            "path": "/",
            "value": {
                "state": "ACTIVE"
            }
        }
    ];
    api.executeHttp('PATCH', this.baseURL + id, activate_attributes, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingPlan.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billingPlan.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billingPlan.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billingPlan.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billingPlan.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billingPlan.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.billing_agreement"></a>[module paypal-rest-sdk.billing_agreement](#apidoc.module.paypal-rest-sdk.billing_agreement)

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.billBalance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>billBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.billBalance)
- description and source-code
```javascript
function billBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/bill-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.bill_balance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>bill_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.bill_balance)
- description and source-code
```javascript
function billBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/bill-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.cancel"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>cancel (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.cancel)
- description and source-code
```javascript
function cancel(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/cancel', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.execute"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>execute (token, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.execute)
- description and source-code
```javascript
function execute(token, data, config, cb) {
    //support case where neither data nor config is provided
    if (typeof data === "function" && arguments.length === 2) {
        cb = data;
        data = {};
    }
    api.executeHttp('POST', this.baseURL + token + '/agreement-execute', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.reactivate"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>reactivate (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.reactivate)
- description and source-code
```javascript
function reactivate(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/re-activate', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.searchTransactions"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>searchTransactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.searchTransactions)
- description and source-code
```javascript
function searchTransactions(id, start_date, end_date, config, cb) {
    var date_range = {
        "start_date": start_date,
        "end_date": end_date
    };
    api.executeHttp('GET', baseURL + id + '/transactions', date_range, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.search_transactions"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>search_transactions (id, start_date, end_date, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.search_transactions)
- description and source-code
```javascript
function searchTransactions(id, start_date, end_date, config, cb) {
    var date_range = {
        "start_date": start_date,
        "end_date": end_date
    };
    api.executeHttp('GET', baseURL + id + '/transactions', date_range, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.setBalance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>setBalance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.setBalance)
- description and source-code
```javascript
function setBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/set-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.set_balance"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>set_balance (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.set_balance)
- description and source-code
```javascript
function setBalance(id, data, config, cb) {
    api.executeHttp('POST', baseURL + id + '/set-balance', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.suspend"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>suspend (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.suspend)
- description and source-code
```javascript
function suspend(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/suspend', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_agreement.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_agreement.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_agreement.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.billing_plan"></a>[module paypal-rest-sdk.billing_plan](#apidoc.module.paypal-rest-sdk.billing_plan)

#### <a name="apidoc.element.paypal-rest-sdk.billing_plan.activate"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>activate (id, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.activate)
- description and source-code
```javascript
function activate(id, config, cb) {
    var activate_attributes = [
        {
            "op": "replace",
            "path": "/",
            "value": {
                "state": "ACTIVE"
            }
        }
    ];
    api.executeHttp('PATCH', this.baseURL + id, activate_attributes, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_plan.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_plan.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_plan.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.billing_plan.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.billing_plan.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.billing_plan.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.capture"></a>[module paypal-rest-sdk.capture](#apidoc.module.paypal-rest-sdk.capture)

#### <a name="apidoc.element.paypal-rest-sdk.capture.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.capture.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.capture.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.capture.refund"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.capture.</span>refund (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.capture.refund)
- description and source-code
```javascript
function refund(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/refund', data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.client"></a>[module paypal-rest-sdk.client](#apidoc.module.paypal-rest-sdk.client)

#### <a name="apidoc.element.paypal-rest-sdk.client.invoke"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.client.</span>invoke (http_method, path, data, http_options_param, cb)](#apidoc.element.paypal-rest-sdk.client.invoke)
- description and source-code
```javascript
function invoke(http_method, path, data, http_options_param, cb) {
    var client = (http_options_param.schema === 'http') ? http : https;

    var request_data = data;

    if (http_method === 'GET') {
        //format object parameters into GET request query string
        if (typeof request_data !== 'string') {
            request_data = querystring.stringify(request_data);
        }
        if (request_data) {
            path = path + "?" + request_data;
            request_data = "";
        }
    } else if (typeof request_data !== 'string') {
        request_data = JSON.stringify(request_data);
    }

    var http_options = {};

    if (http_options_param) {

        http_options = JSON.parse(JSON.stringify(http_options_param));

        if (!http_options.headers) {
            http_options.headers = {};
        }
        http_options.path = path;
        http_options.method = http_method;
        if (request_data) {
            http_options.headers['Content-Length'] = Buffer.byteLength(request_data, 'utf-8');
        }

        if (!http_options.headers.Accept) {
            http_options.headers.Accept = 'application/json';
        }

        if (!http_options.headers['Content-Type']) {
            http_options.headers['Content-Type'] = 'application/json';
        }

        if (http_method === 'POST' && !http_options.headers['PayPal-Request-Id']) {
            http_options.headers['PayPal-Request-Id'] = uuid.v4();
        }

        http_options.headers['User-Agent'] = configuration.userAgent;
        http_options.withCredentials = false;
    }

    // Enable full request response logging in development/non-production environment only
    if (configuration.default_options.mode !== 'live' && process.env.NODE_ENV === 'development') {
        console.dir(JSON.stringify(http_options.headers));
        console.dir(request_data);
    }

    //PCI compliance
    if (process.versions !== undefined && process.versions.openssl !== undefined && semver.lt(process.versions.openssl.slice(0,
5), '1.0.1')) {
        console.warn('WARNING: openssl version ' + process.versions.openssl + ' detected. Per PCI Security Council mandate (https
://github.com/paypal/TLS-update), you MUST update to the latest security library.');
    }

    var req = client.request(http_options);
    req.on('error', function (e) {
        console.log('problem with request: ' + e.message);
        cb(e, null);
    });

    req.on('response', function (res) {
        var response = '';
        //do not setEndcoding with browserify
        if (res.setEncoding) {
            res.setEncoding('utf8');
        }

        res.on('data', function (chunk) {
            response += chunk;
        });

        res.on('end', function () {
            var err = null;

            try {
                //TURN NODE_ENV to development to get access to paypal-debug-id
                //for questions to merchant technical services.
                if (res.headers['paypal-debug-id'] !== undefined && process.env.NODE_ENV === 'development') {
                    console.log('paypal-debug-id: ' + res.headers['paypal-debug-id']);

                    if (configuration.default_options.mode !== 'live') {
                        console.dir(JSON.stringify(res.headers));
                        console.dir(response);
                    }
                }

                //Set response to be parsed JSON object if data received is json
                //expect that content-type header has application/json when it
                //returns data
                if (typeof res.headers['content-type'] === "string" &&
                    res.headers['content-type'].match(/^application\/json(?:;.*)?$/) !== null) {
                    response = JSON.parse(response);
                }
                //Set response to an empty object if no data was received
                if (response === '') {
                    response = {};
                }
                response.httpStatusCode = res.statusCode;
            } catch (e) {
                err = new Error('Invalid JSON Response Rec ...
```
- example usage
```shell
...
    headers: utils.merge({
        'Authorization': basicAuthString,
        'Accept': 'application/json',
        'Content-Type': 'application/x-www-form-urlencoded'
    }, configuration.default_options.headers, true)
};

client.invoke('POST', '/v1/oauth2/token', payload, http_options, function (err, res) {
    var token = null;
    if (res) {
        if (!config.authorization_code && !config.refresh_token) {
            var seconds = new Date().getTime() / 1000;
            token_persist[config.client_id] = res;
            token_persist[config.client_id].created_at = seconds;
        }
...
```



# <a name="apidoc.module.paypal-rest-sdk.creditCard"></a>[module paypal-rest-sdk.creditCard](#apidoc.module.paypal-rest-sdk.creditCard)

#### <a name="apidoc.element.paypal-rest-sdk.creditCard.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.creditCard.del"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.del)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.creditCard.delete"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.delete)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.creditCard.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.creditCard.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.creditCard.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.creditCard.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.creditCard.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.credit_card"></a>[module paypal-rest-sdk.credit_card](#apidoc.module.paypal-rest-sdk.credit_card)

#### <a name="apidoc.element.paypal-rest-sdk.credit_card.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.credit_card.del"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.del)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.credit_card.delete"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.delete)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.credit_card.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.credit_card.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.credit_card.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.credit_card.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.credit_card.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.generate"></a>[module paypal-rest-sdk.generate](#apidoc.module.paypal-rest-sdk.generate)

#### <a name="apidoc.element.paypal-rest-sdk.generate.mixin"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.generate.</span>mixin (destObject, operations)](#apidoc.element.paypal-rest-sdk.generate.mixin)
- description and source-code
```javascript
function mixin(destObject, operations) {
    operations.forEach(function (property) {
        destObject[property] = restFunctions[property];
    });
    return destObject;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.invoice"></a>[module paypal-rest-sdk.invoice](#apidoc.module.paypal-rest-sdk.invoice)

#### <a name="apidoc.element.paypal-rest-sdk.invoice.cancel"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>cancel (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.cancel)
- description and source-code
```javascript
function cancel(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/cancel', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.del"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.del)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.delete"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.delete)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.deleteExternalPayment"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>deleteExternalPayment (invoiceId, transactionId, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.deleteExternalPayment)
- description and source-code
```javascript
function deleteExternalPayment(invoiceId, transactionId, config, cb) {
    api.executeHttp('DELETE', this.baseURL + invoiceId + '/payment-records/' + transactionId, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.deleteExternalRefund"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>deleteExternalRefund (invoiceId, transactionId, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.deleteExternalRefund)
- description and source-code
```javascript
function deleteExternalRefund(invoiceId, transactionId, config, cb) {
    api.executeHttp('DELETE', this.baseURL + invoiceId + '/refund-records/' + transactionId, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.generateNumber"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>generateNumber (config, cb)](#apidoc.element.paypal-rest-sdk.invoice.generateNumber)
- description and source-code
```javascript
function generateNumber(config, cb) {
    api.executeHttp("POST", this.baseURL + '/next-invoice-number', {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.qrCode"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>qrCode (id, height, width, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.qrCode)
- description and source-code
```javascript
function qrCode(id, height, width, config, cb) {
    var image_attributes = {
        "height": height,
        "width": width
    };
    api.executeHttp('GET', this.baseURL + id + '/qr-code', image_attributes, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.recordPayment"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>recordPayment (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.recordPayment)
- description and source-code
```javascript
function recordPayment(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/record-payment', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.recordRefund"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>recordRefund (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.recordRefund)
- description and source-code
```javascript
function recordRefund(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/record-refund', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.remind"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>remind (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.remind)
- description and source-code
```javascript
function remind(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/remind', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.search"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>search (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.search)
- description and source-code
```javascript
function search(data, config, cb) {
    api.executeHttp('POST', '/v1/invoicing/search', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.send"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>send (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.send)
- description and source-code
```javascript
function send(id, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/send', {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoice.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoice.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoice.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PUT', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.invoiceTemplate"></a>[module paypal-rest-sdk.invoiceTemplate](#apidoc.module.paypal-rest-sdk.invoiceTemplate)

#### <a name="apidoc.element.paypal-rest-sdk.invoiceTemplate.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.invoiceTemplate.delete"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.delete)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoiceTemplate.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.invoiceTemplate.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.invoiceTemplate.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.invoiceTemplate.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.invoiceTemplate.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PUT', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.openIdConnect"></a>[module paypal-rest-sdk.openIdConnect](#apidoc.module.paypal-rest-sdk.openIdConnect)

#### <a name="apidoc.element.paypal-rest-sdk.openIdConnect.authorizeUrl"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>authorizeUrl (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.authorizeUrl)
- description and source-code
```javascript
function authorizeUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    //Use mode provided, live or sandbox to construct authorize_url, sandbox is default
    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/signin/authorize' || config.authorize_url;

    data = utils.merge({
        'client_id': getClientId(config),
        'scope': 'openid',
        'response_type': 'code',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
...
// OpenID configuration
paypal.configure({
  'openid_client_id': 'CLIENT_ID',
  'openid_client_secret': 'CLIENT_SECRET',
  'openid_redirect_uri': 'http://example.com' });

// Authorize url
paypal.openIdConnect.authorizeUrl({'scope': 'openid profile'});

// Get tokeninfo with Authorize code
paypal.openIdConnect.tokeninfo.create("Replace with authorize code", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get tokeninfo with Refresh code
...
```

#### <a name="apidoc.element.paypal-rest-sdk.openIdConnect.authorize_url"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>authorize_url (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.authorize_url)
- description and source-code
```javascript
function authorizeUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    //Use mode provided, live or sandbox to construct authorize_url, sandbox is default
    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/signin/authorize' || config.authorize_url;

    data = utils.merge({
        'client_id': getClientId(config),
        'scope': 'openid',
        'response_type': 'code',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.openIdConnect.logoutUrl"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>logoutUrl (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.logoutUrl)
- description and source-code
```javascript
function logoutUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/webapps/auth/protocol/openidconnect/v1/endsession' || config
.logout_url;

    if (typeof data === 'string') {
        data = { 'id_token': data };
    }

    data = utils.merge({
        'logout': 'true',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
...

    // Get userinfo with Access code
    paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
      console.log(userinfo);
    });

    // Logout url
    paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
    '''

## Running Samples
Instructions for running samples are located in the [sample directory](/samples).

## Running Tests
To run the test suite first invoke the following command within the repo
...
```

#### <a name="apidoc.element.paypal-rest-sdk.openIdConnect.logout_url"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.</span>logout_url (data, config)](#apidoc.element.paypal-rest-sdk.openIdConnect.logout_url)
- description and source-code
```javascript
function logoutUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/webapps/auth/protocol/openidconnect/v1/endsession' || config
.logout_url;

    if (typeof data === 'string') {
        data = { 'id_token': data };
    }

    data = utils.merge({
        'logout': 'true',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.openIdConnect.tokeninfo"></a>[module paypal-rest-sdk.openIdConnect.tokeninfo](#apidoc.module.paypal-rest-sdk.openIdConnect.tokeninfo)

#### <a name="apidoc.element.paypal-rest-sdk.openIdConnect.tokeninfo.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.tokeninfo.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.openIdConnect.tokeninfo.create)
- description and source-code
```javascript
create = function (data, config, cb) {
    if (typeof data === 'string') {
        data = { 'code': data };
    }
    data.grant_type = 'authorization_code';
    tokenInfoRequest(data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.openIdConnect.tokeninfo.refresh"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.tokeninfo.</span>refresh (data, config, cb)](#apidoc.element.paypal-rest-sdk.openIdConnect.tokeninfo.refresh)
- description and source-code
```javascript
refresh = function (data, config, cb) {
    if (typeof data === 'string') {
        data = { 'refresh_token': data };
    }
    data.grant_type = 'refresh_token';
    tokenInfoRequest(data, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Authorize code
paypal.openIdConnect.tokeninfo.create("Replace with authorize code", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});
...
```



# <a name="apidoc.module.paypal-rest-sdk.openIdConnect.userinfo"></a>[module paypal-rest-sdk.openIdConnect.userinfo](#apidoc.module.paypal-rest-sdk.openIdConnect.userinfo)

#### <a name="apidoc.element.paypal-rest-sdk.openIdConnect.userinfo.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openIdConnect.userinfo.</span>get (data, config, cb)](#apidoc.element.paypal-rest-sdk.openIdConnect.userinfo.get)
- description and source-code
```javascript
function userInfoRequest(data, config, cb) {
    if (typeof config === 'function') {
        cb = config;
        config = configuration.default_options;
    } else if (!config) {
        config = configuration.default_options;
    }

    if (typeof data === 'string') {
        data = { 'access_token': data };
    }

    data = utils.merge({
        'schema': 'openid'
    }, data);

    openIdConnectRequest('/v1/identity/openidconnect/userinfo', data, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```



# <a name="apidoc.module.paypal-rest-sdk.openid_connect"></a>[module paypal-rest-sdk.openid_connect](#apidoc.module.paypal-rest-sdk.openid_connect)

#### <a name="apidoc.element.paypal-rest-sdk.openid_connect.authorizeUrl"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>authorizeUrl (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.authorizeUrl)
- description and source-code
```javascript
function authorizeUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    //Use mode provided, live or sandbox to construct authorize_url, sandbox is default
    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/signin/authorize' || config.authorize_url;

    data = utils.merge({
        'client_id': getClientId(config),
        'scope': 'openid',
        'response_type': 'code',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
...
// OpenID configuration
paypal.configure({
  'openid_client_id': 'CLIENT_ID',
  'openid_client_secret': 'CLIENT_SECRET',
  'openid_redirect_uri': 'http://example.com' });

// Authorize url
paypal.openIdConnect.authorizeUrl({'scope': 'openid profile'});

// Get tokeninfo with Authorize code
paypal.openIdConnect.tokeninfo.create("Replace with authorize code", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get tokeninfo with Refresh code
...
```

#### <a name="apidoc.element.paypal-rest-sdk.openid_connect.authorize_url"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>authorize_url (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.authorize_url)
- description and source-code
```javascript
function authorizeUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    //Use mode provided, live or sandbox to construct authorize_url, sandbox is default
    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/signin/authorize' || config.authorize_url;

    data = utils.merge({
        'client_id': getClientId(config),
        'scope': 'openid',
        'response_type': 'code',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.openid_connect.logoutUrl"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>logoutUrl (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.logoutUrl)
- description and source-code
```javascript
function logoutUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/webapps/auth/protocol/openidconnect/v1/endsession' || config
.logout_url;

    if (typeof data === 'string') {
        data = { 'id_token': data };
    }

    data = utils.merge({
        'logout': 'true',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
...

    // Get userinfo with Access code
    paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
      console.log(userinfo);
    });

    // Logout url
    paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
    '''

## Running Samples
Instructions for running samples are located in the [sample directory](/samples).

## Running Tests
To run the test suite first invoke the following command within the repo
...
```

#### <a name="apidoc.element.paypal-rest-sdk.openid_connect.logout_url"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.</span>logout_url (data, config)](#apidoc.element.paypal-rest-sdk.openid_connect.logout_url)
- description and source-code
```javascript
function logoutUrl(data, config) {
    config = config || configuration.default_options;
    data   = data || {};

    var url = 'https://www.' + utils.getDefaultEndpoint(config.mode) + '/webapps/auth/protocol/openidconnect/v1/endsession' || config
.logout_url;

    if (typeof data === 'string') {
        data = { 'id_token': data };
    }

    data = utils.merge({
        'logout': 'true',
        'redirect_uri': getRedirectUri(config)
    }, data);

    return url + '?' + querystring.stringify(data);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.openid_connect.tokeninfo"></a>[module paypal-rest-sdk.openid_connect.tokeninfo](#apidoc.module.paypal-rest-sdk.openid_connect.tokeninfo)

#### <a name="apidoc.element.paypal-rest-sdk.openid_connect.tokeninfo.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.tokeninfo.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.openid_connect.tokeninfo.create)
- description and source-code
```javascript
create = function (data, config, cb) {
    if (typeof data === 'string') {
        data = { 'code': data };
    }
    data.grant_type = 'authorization_code';
    tokenInfoRequest(data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.openid_connect.tokeninfo.refresh"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.tokeninfo.</span>refresh (data, config, cb)](#apidoc.element.paypal-rest-sdk.openid_connect.tokeninfo.refresh)
- description and source-code
```javascript
refresh = function (data, config, cb) {
    if (typeof data === 'string') {
        data = { 'refresh_token': data };
    }
    data.grant_type = 'refresh_token';
    tokenInfoRequest(data, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Authorize code
paypal.openIdConnect.tokeninfo.create("Replace with authorize code", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});
...
```



# <a name="apidoc.module.paypal-rest-sdk.openid_connect.userinfo"></a>[module paypal-rest-sdk.openid_connect.userinfo](#apidoc.module.paypal-rest-sdk.openid_connect.userinfo)

#### <a name="apidoc.element.paypal-rest-sdk.openid_connect.userinfo.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.openid_connect.userinfo.</span>get (data, config, cb)](#apidoc.element.paypal-rest-sdk.openid_connect.userinfo.get)
- description and source-code
```javascript
function userInfoRequest(data, config, cb) {
    if (typeof config === 'function') {
        cb = config;
        config = configuration.default_options;
    } else if (!config) {
        config = configuration.default_options;
    }

    if (typeof data === 'string') {
        data = { 'access_token': data };
    }

    data = utils.merge({
        'schema': 'openid'
    }, data);

    openIdConnectRequest('/v1/identity/openidconnect/userinfo', data, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```



# <a name="apidoc.module.paypal-rest-sdk.order"></a>[module paypal-rest-sdk.order](#apidoc.module.paypal-rest-sdk.order)

#### <a name="apidoc.element.paypal-rest-sdk.order.authorize"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>authorize (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.order.authorize)
- description and source-code
```javascript
function authorize(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/authorize', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.order.capture"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>capture (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.order.capture)
- description and source-code
```javascript
function capture(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/capture', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.order.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.order.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.order.void"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.order.</span>void (id, config, cb)](#apidoc.element.paypal-rest-sdk.order.void)
- description and source-code
```javascript
function voidOrder(id, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/do-void', {}, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.payment"></a>[module paypal-rest-sdk.payment](#apidoc.module.paypal-rest-sdk.payment)

#### <a name="apidoc.element.paypal-rest-sdk.payment.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.payment.execute"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>execute (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.execute)
- description and source-code
```javascript
function execute(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/execute', data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.payment.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.payment.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.payment.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.payment.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payment.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.payment.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.payout"></a>[module paypal-rest-sdk.payout](#apidoc.module.paypal-rest-sdk.payout)

#### <a name="apidoc.element.paypal-rest-sdk.payout.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payout.</span>create (data, sync_mode, config, cb)](#apidoc.element.paypal-rest-sdk.payout.create)
- description and source-code
```javascript
function create(data, sync_mode, config, cb) {
    cb = (typeof sync_mode === 'function') ? sync_mode : cb;
    sync_mode = (typeof sync_mode === 'string' && sync_mode === 'true') ? 'true' : 'false';
    api.executeHttp('POST', this.baseURL + "?" + "sync_mode=" + sync_mode, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.payout.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payout.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.payout.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```



# <a name="apidoc.module.paypal-rest-sdk.payoutItem"></a>[module paypal-rest-sdk.payoutItem](#apidoc.module.paypal-rest-sdk.payoutItem)

#### <a name="apidoc.element.paypal-rest-sdk.payoutItem.cancel"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payoutItem.</span>cancel (id, config, cb)](#apidoc.element.paypal-rest-sdk.payoutItem.cancel)
- description and source-code
```javascript
function cancel(id, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/cancel', {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.payoutItem.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.payoutItem.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.payoutItem.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```



# <a name="apidoc.module.paypal-rest-sdk.refund"></a>[module paypal-rest-sdk.refund](#apidoc.module.paypal-rest-sdk.refund)

#### <a name="apidoc.element.paypal-rest-sdk.refund.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.refund.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.refund.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```



# <a name="apidoc.module.paypal-rest-sdk.sale"></a>[module paypal-rest-sdk.sale](#apidoc.module.paypal-rest-sdk.sale)

#### <a name="apidoc.element.paypal-rest-sdk.sale.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.sale.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.sale.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.sale.refund"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.sale.</span>refund (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.sale.refund)
- description and source-code
```javascript
function refund(id, data, config, cb) {
    api.executeHttp('POST', this.baseURL + id + '/refund', data, config, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.paypal-rest-sdk.utils"></a>[module paypal-rest-sdk.utils](#apidoc.module.paypal-rest-sdk.utils)

#### <a name="apidoc.element.paypal-rest-sdk.utils.checkExpiredToken"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>checkExpiredToken (token_hash)](#apidoc.element.paypal-rest-sdk.utils.checkExpiredToken)
- description and source-code
```javascript
function checkExpiredToken(token_hash) {
    var delta = (new Date().getTime() / 1000) - token_hash.created_at;
    return (delta < token_hash.expires_in) ? false : true;
}
```
- example usage
```shell
...
    http_options.headers['Paypal-Client-Metadata-Id'] = http_options.client_metadata_id;
}
else if (http_options.correlation_id) {
    http_options.headers['Paypal-Client-Metadata-Id'] = http_options.correlation_id;
}

// If client_id exists with an unexpired token and a refresh token is not provided, reuse cached token
if (http_options.client_id in token_persist && !utils.checkExpiredToken(token_persist[http_options.client_id]) && !http_options.
refresh_token) {
    http_options.headers.Authorization = "Bearer " + token_persist[http_options.client_id].access_token;
    client.invoke(http_method, path, data, http_options, function (error, response) {
        // Don't reprompt already authenticated user for login by updating Authorization header
        // if token expires
        if (error && error.httpStatusCode === 401 && http_options.client_id && http_options.headers.Authorization) {
            http_options.headers.Authorization = null;
            updateToken(http_options, cb, retryInvoke);
...
```

#### <a name="apidoc.element.paypal-rest-sdk.utils.getDefaultApiEndpoint"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>getDefaultApiEndpoint (mode)](#apidoc.element.paypal-rest-sdk.utils.getDefaultApiEndpoint)
- description and source-code
```javascript
function getDefaultApiEndpoint(mode) {
    var api = (typeof mode === "string" && mode === "security-test-sandbox") ? "test-api." : "api.";
    return api + getDefaultEndpoint(mode);
}
```
- example usage
```shell
...
    payload = 'grant_type=refresh_token&refresh_token=' + config.refresh_token;
}

var basicAuthString = 'Basic ' + new Buffer(config.client_id + ':' + config.client_secret).toString('base64');

var http_options = {
    schema: config.schema || configuration.default_options.schema,
    host: utils.getDefaultApiEndpoint(config.mode) || config.host || configuration.default_options.host,
    port: config.port || configuration.default_options.port,
    headers: utils.merge({
        'Authorization': basicAuthString,
        'Accept': 'application/json',
        'Content-Type': 'application/x-www-form-urlencoded'
    }, configuration.default_options.headers, true)
};
...
```

#### <a name="apidoc.element.paypal-rest-sdk.utils.getDefaultEndpoint"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>getDefaultEndpoint (mode)](#apidoc.element.paypal-rest-sdk.utils.getDefaultEndpoint)
- description and source-code
```javascript
function getDefaultEndpoint(mode) {
    return (typeof mode === "string" && mode === "live") ? "paypal.com" : "sandbox.paypal.com";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.utils.merge"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.utils.</span>merge (obj1, obj2, appendOnly)](#apidoc.element.paypal-rest-sdk.utils.merge)
- description and source-code
```javascript
function merge(obj1, obj2, appendOnly) {

    //Handle invalid arguments
    if (obj1 === null || typeof obj1 !== "object") {
        throw new TypeError("merge() - first parameter has to be an object, not " + typeof obj1 + ".");
    }

    if (obj2 === null || typeof obj2 !== "object") {
        throw new TypeError("merge() - first parameter has to be an object, not " + typeof obj2 + ".");
    }

    if (isArray(obj1) || isArray(obj2)) {
        throw new TypeError("merge() - Unsupported for arrays.");
    }

    for (var k in obj2) {
        var obj1Val, obj2Val = obj2[k];
        if (hasOwn.call(obj1, k)) {
            if (!appendOnly) {
                obj1Val = obj1[k];
                if (obj1Val !== null && typeof obj1Val === "object" &&
                        obj2Val !== null && typeof obj2Val === "object") {
                    merge(obj1Val, obj2Val);
                }
                else {
                    obj1[k] = clone(obj2Val);
                }
            }
        }
        else {
            obj1[k] = clone(obj2Val);
        }
    }
    return obj1;
}
```
- example usage
```shell
...
* Set up configuration globally such as client_id and client_secret,
* by merging user provided configurations otherwise use default settings
* @param  {Object} options Configuration parameters passed as object
* @return {undefined}
*/
var configure = exports.configure = function configure(options) {
   if (options !== undefined && typeof options === 'object') {
       configuration.default_options = utils.merge(configuration.default_options, options);
   }
};

/**
* Generate new access token by making a POST request to /oauth2/token by
* exchanging base64 encoded client id/secret pair or valid refresh token.
*
...
```



# <a name="apidoc.module.paypal-rest-sdk.webProfile"></a>[module paypal-rest-sdk.webProfile](#apidoc.module.paypal-rest-sdk.webProfile)

#### <a name="apidoc.element.paypal-rest-sdk.webProfile.create"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>create (data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.create)
- description and source-code
```javascript
function create(data, config, cb) {
    api.executeHttp('POST', this.baseURL, data, config, cb);
}
```
- example usage
```shell
...
  "expire_month": "11",
  "expire_year": "2018",
  "cvv2": "123",
  "first_name": "Joe",
  "last_name": "Shopper"
};

paypal.creditCard.create(card_data, function(error, credit_card){
  if (error) {
    console.log(error);
    throw error;
  } else {
    console.log("Create Credit-Card Response");
    console.log(credit_card);
  }
...
```

#### <a name="apidoc.element.paypal-rest-sdk.webProfile.del"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>del (id, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.del)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.webProfile.delete"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>delete (id, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.delete)
- description and source-code
```javascript
function del(id, config, cb) {
    api.executeHttp('DELETE', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.webProfile.get"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>get (id, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.get)
- description and source-code
```javascript
function get(id, config, cb) {
    api.executeHttp('GET', this.baseURL + id, {}, config, cb);
}
```
- example usage
```shell
...

// Get tokeninfo with Refresh code
paypal.openIdConnect.tokeninfo.refresh("Replace with refresh_token", function(error, tokeninfo){
  console.log(tokeninfo);
});

// Get userinfo with Access code
paypal.openIdConnect.userinfo.get("Replace with access_code", function(error, userinfo){
  console.log(userinfo);
});

// Logout url
paypal.openIdConnect.logoutUrl("Replace with tokeninfo.id_token");
'''
...
```

#### <a name="apidoc.element.paypal-rest-sdk.webProfile.list"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>list (data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.list)
- description and source-code
```javascript
function list(data, config, cb) {
    if (typeof data === 'function') {
        config = data;
        data = {};
    }
    api.executeHttp('GET', this.baseURL, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.webProfile.replace"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>replace (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.replace)
- description and source-code
```javascript
function replace(id, data, config, cb) {
    api.executeHttp('PATCH', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.paypal-rest-sdk.webProfile.update"></a>[function <span class="apidocSignatureSpan">paypal-rest-sdk.webProfile.</span>update (id, data, config, cb)](#apidoc.element.paypal-rest-sdk.webProfile.update)
- description and source-code
```javascript
function update(id, data, config, cb) {
    api.executeHttp('PUT', this.baseURL + id, data, config, cb);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
