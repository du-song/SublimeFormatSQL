## Summary

FormatSQL formats long SQL statement to a more readable form by using [python-sqlparse library](http://code.google.com/p/python-sqlparse/).


## How to Use

select sql and click menu Selection -> Format -> SQL


### Configure key binding

add the following line to keymap settings

	{ "keys": ["super+k", "super+s"], "command": "format_sql" },


## Example

Original:

	select a,b from foo join bar on val1 = val2 where id = 123 and cd = 99;

Formated:

	SELECT a,
	       b
	FROM foo
	JOIN bar ON val1 = val2
	WHERE id = 123
	    AND cd = 99;

## License

[python-sqlparse library](http://code.google.com/p/python-sqlparse/) and this code are both on [2-clauses BSD](http://www.opensource.org/licenses/bsd-license.php)