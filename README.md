### [👉👉👉♥♥点此进入♥观看入口👈👈👈](https://mrddrm.github.io/91.html)
<br></br><br></br><br></br>
self.users[self.current_user]['records'].append(record)
        self.save_data()
        return True, "记录成功"
    
    def record_health_metric(self, metric_type: str, value: float, date: str = None):
        """记录健康指标"""
        if not self.current_user:
            return False, "请先登录"
        
        if not date:
            date = datetime.datetime.now().strftime('%Y-%m-%d')
        
        metric = {
            'type': metric_type,  # 如 'weight', 'blood_pressure', 'blood_sugar'
            'value': value,
            'date': date
        }
