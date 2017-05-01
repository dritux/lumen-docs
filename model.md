## Docs Model



#### Before save set null fields

```
public static function boot() {
	parent::boot();

	static::saving(function($model){
		foreach ($model->attributes as $key => $value) {
			if($value !== 0) {
			$model->{$key} = empty($value) ? null : $value;
			}
		}
	});
}
```

#### Joins

```
public static function resources($user_id){
	$result = UserGroup::join('user_group_permission', 'user_group.id', '=', 'user_group_permission.user_group_id')
	->join('user_permission', 'user_group_permission.user_permission_id', '=', 'user_permission.id')
	->select('user_group.name', 'user_permission.resource')
	->getQuery() 
	->get();
	return $result;
}
```
