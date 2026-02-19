A schedule is *cascade less* if no transaction reads a data item that was written by an uncommitted transaction.

A schedule is *strict* is no transaction reads or overwrites a data item that is written by an uncommitted transaction. 
