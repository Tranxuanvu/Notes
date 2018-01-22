## Field type jsonb
- To pass data for `info` has type is jsonb, need add merge data in controller like this:
```
  params.require(:job).permit(:name, :category).merge(info: params[:job][:info])
```
