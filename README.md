# openam-agent-cache
Abstract cache for the OpenAM Policy Agent for NodeJS

Implement this class to use your own cache with any backed with the
[node-openam-policy-agent](https://github.com/zoltantarcsay/node-openam-agent)

## API docs

<a name="Cache"></a>

### *Cache*
**Kind**: global abstract class  

* *[Cache](#Cache)*
    * *[new Cache()](#new_Cache_new)*
    * *[.get(key)](#Cache+get) ⇒ <code>Promise</code>*
    * *[.put(key, value)](#Cache+put) ⇒ <code>Promise</code>*
    * *[.remove(key)](#Cache+remove) ⇒ <code>Promise</code>*

<a name="new_Cache_new"></a>

#### *new Cache()*
Abstract Cache class

<a name="Cache+get"></a>

#### *cache.get(key) ⇒ <code>Promise</code>*
Get a single cached item
If the entry is not found, reject

**Kind**: instance method of <code>[Cache](#Cache)</code>  

| Param | Type |
| --- | --- |
| key | <code>string</code> | 

<a name="Cache+put"></a>

#### *cache.put(key, value) ⇒ <code>Promise</code>*
Store a single cached item (overwrites existing)

**Kind**: instance method of <code>[Cache](#Cache)</code>  

| Param | Type |
| --- | --- |
| key | <code>string</code> | 
| value | <code>\*</code> | 

<a name="Cache+remove"></a>

#### *cache.remove(key) ⇒ <code>Promise</code>*
Remove a single cached item

**Kind**: instance method of <code>[Cache](#Cache)</code>  

| Param | Type |
| --- | --- |
| key | <code>string</code> | 


