
* 請寫一段 Ruby 程式，把 `[1, 3, 5, 7, 9]` 變成 `[2, 4, 6, 8, 10]`
```
num=[1,3,5,7,9]
p num.map{|sum|sum+1}
```

* 請印出在 1 到 2000 中，可以被 4 整除，但不能 100 整除，但又要可以被 400 整除的數字。(潤年計算公式)
```
p (1..2000).to_a.select {|ys|  
	(ys % 400) == 0 or (ys % 4 ==0 and ys % 100 != 0)
}
```

* 請印出在 1 到 100 中所有單數的總和。
```
p (1..100).to_a.select{|nuodd| nuodd.odd?}.inject(:+)
```


* 請試著解釋什麼是 Symbol。
```
如果使用symbol,則object.ID相同
