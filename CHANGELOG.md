Meteor + Mongo Transactions
===========================

### v1.x

- Explore Operational Transform options
- Look into support for `{multi:true}`
- Support for `upsert`
- Possible support for locking documents used in pending transactions

### v1.0

- Refactor and document code for better maintainability
- Add/improve support for other/existing mongo operators  
- Complete test coverage and security audit

### vNext

- More comprehensive test coverage

### v0.7.5

- Fixes for a number of issues, the chief one being a broken rollback mechanism
- A small change in which auto committed insert transactions are not processed client side, but are sent to the server for writes, like  other transactions in `tx.start() ... tx.commit()` blocks, removing the need for allow/deny rules for inserts

### v0.7.0

- First release using new storage format for transactions and having db state recovery options

### v0.6.21

- Last stable(ish) release using naive/optimistic transactions with no db state recoverability