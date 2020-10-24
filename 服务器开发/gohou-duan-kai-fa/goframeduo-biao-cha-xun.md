# GoFrame多表查询
<!-- 
```go
func GetAllHeroOrderByPage(pageIndex int, pageTotal int, orderBy string, where string, args ...interface{}) (r []*modelLottoHero.LottoHeroOrderEntity) {
    sqlString := ""
    lottos := ([]modelLottoHero.LottoHeroConfigEntity)(nil)
    lottoErr := g.DB().Table("lotto_hero_config").Order("id ASC").Structs(&lottos)
    if lottoErr != nil {
        glog.Error(g.Map{"area": "service", "method": "GetAllHeroOrderByPage", "error": lottoErr.Error()})
        return
    }
    totalArgs := garray.New()
    for i := 0; i < len(lottos); i++ {
        tempSql := "SELECT * FROM " + getTableNameOrder(gconv.Int16(lottos[i].ID))
        tempSql += " where user_id = ?"
        tempSql += " and (bet_time between ? and ?)"
        if len(args) > 3 && args[3] != -1 {
            tempSql += " and status = ?"
            totalArgs.Merge(args)
        } else {
            totalArgs.Merge(args).PopRight()
        }
        if !g.IsEmpty(sqlString) {
            sqlString += " UNION " + tempSql
        } else {
            sqlString += tempSql
        }
    }
    if !g.IsEmpty(orderBy) {
        sqlString += " ORDER BY " + orderBy
    }
    sqlString += " LIMIT " + gconv.String(pageTotal) + " OFFSET " + gconv.String((pageIndex-1)*pageIndex)
    result, _ := g.DB().GetAll(sqlString, totalArgs.Slice())
    err := result.Structs(&r)
    if err != nil {
        glog.Error(g.Map{"area": "service", "method": "GetAllHeroOrderByPage", "error": err.Error()})
    }
    return
}
```
-->



