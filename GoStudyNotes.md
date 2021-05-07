在同一个文件夹下 不能有两个文件具有两个不同的package
文件的package名字和文件夹的名字 可以不一样 但是最好一样


	//我服了 groups 应该是关键字 做表名不行 要用反引号引起来
    为Raw 不是 finish 而是 chainable 适用于查找

可以把select的数据直接 存到 数组里
    var gids []string
	tx.Raw("select gid from invitations where cid=? and sid=? and group_status <> 2", cid, sid).Scan(&gids)