# openam-agent-cache
Abstract cache for the OpenAM Policy Agent for NodeJS

Implement this class to use your own cache with any backed with the
[node-openam-policy-agent](https://github.com/ForgeRock/node-openam-agent)

# API Docs

<a name="Cache"></a>

## *Cache*
**Kind**: global abstract class  

* *[Cache](#Cache)*
    * *[new Cache()](#new_Cache_new)*
    * *[.get(key)](#Cache+get) ⇒ <code>Promise</code>*
    * *[.put(key, value)](#Cache+put) ⇒ <code>Promise</code>*
    * *[.remove(key)](#Cache+remove) ⇒ <code>Promise</code>*
    * *[.quit()](#Cache+quit) ⇒ <code>Promise</code>*

<a name="new_Cache_new"></a>

### *new Cache()*
Abstract Cache class

<a name="Cache+get"></a>

### *cache.get(key) ⇒ <code>Promise</code>*
Get a single cached item
If the entry is not found, reject

**Kind**: instance method of <code>[Cache](#Cache)</code>  

| Param | Type |
| --- | --- |
| key | <code>string</code> | 

<a name="Cache+put"></a>

### *cache.put(key, value) ⇒ <code>Promise</code>*
Store a single cached item (overwrites existing)

**Kind**: instance method of <code>[Cache](#Cache)</code>  

| Param | Type |
| --- | --- |
| key | <code>string</code> | 
| value | <code>\*</code> | 

<a name="Cache+remove"></a>

### *cache.remove(key) ⇒ <code>Promise</code>*
Remove a single cached item

**Kind**: instance method of <code>[Cache](#Cache)</code>  

| Param | Type |
| --- | --- |
| key | <code>string</code> | 

<a name="Cache+quit"></a>

### *cache.quit() ⇒ <code>Promise</code>*
Closes the client connection

**Kind**: instance method of <code>[Cache](#Cache)</code>  

## DISCLAIMER

The sample code described herein is provided on an "as is" basis, without warranty of any kind, to the fullest extent permitted by law. ForgeRock does not warrant or guarantee the individual success developers may have in implementing the sample code on their development platforms or in production configurations.

ForgeRock does not warrant, guarantee or make any representations regarding the use, results of use, accuracy, timeliness or completeness of any data or information relating to the sample code. ForgeRock disclaims all warranties, expressed or implied, and in particular, disclaims all warranties of merchantability, and warranties related to the code, or any service or software related thereto.

ForgeRock shall not be liable for any direct, indirect or consequential damages or costs of any type arising out of any action taken by you or others related to the sample code.