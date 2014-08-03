# Former Snippets for Sublime Text

These snippets are for methods in [Former] (https://github.com/Anahkiasen/former) which is a powerful form builder package for [Laravel] (http://laravel.com) and other frameworks.

##Installation
Clone this repository into your Packages folder:

    git clone https://github.com/andrewmile/former-snippets.git

Or download the zip file and unzip it into your Sublime Packages/User folder

##Usage
Type the snippet shortcut inside of a Blade file and press the tab key.

##Snippets
<table>
	<tr>
		<th>Snippet</th>
		<th>Trigger</th>
		<th>Output</th>
	</tr>
	<tr>
		<td>Form</td>
		<td>fo</td>
		<td>{{ Former::open()->route('route')->id('form') }}

				Former::populate(Input::old());

				

			{{ Former::close() }}</td>
	</tr>
	<tr>
		<td>Text</td>
		<td>ft</td>
		<td>{{ Former::sm_text('field') }}</td>
	</tr>
	<tr>
		<td>Text Area</td>
		<td>fta</td>
		<td>{{ Former::textArea('field') }}</td>
	</tr>
	<tr>
		<td>Password</td>
		<td>fp</td>
		<td>{{ Former::sm_password('password') }}</td>
	</tr>
	<tr>
		<td>Select</td>
		<td>fs</td>
		<td>{{ Former::sm_select('field')->options($options) }}</td>
	</tr>
	<tr>
		<td>Inline Radios</td>
		<td>fr</td>
		<td>{{ Former::inline_radios('field')
				->radios([
					'Label One' => ['name' => 'field', 'value' => 'value one'],
					'Label Two' => ['name' => 'field', 'value' => 'value two']
				]) }}</td>
	</tr>
	<tr>
		<td>Hidden</td>
		<td>fh</td>
		<td>{{ Former::hidden('field')->value($value) }}</td>
	</tr>
	<tr>
		<td>Label</td>
		<td>fl</td>
		<td>->label('label')</td>
	</tr>
	<tr>
		<td>Class</td>
		<td>fc</td>
		<td>->addClass('class')</td>
	</tr>
	<tr>
		<td>Group Class</td>
		<td>fgc</td>
		<td>->addGroupClass('class')</td>
	</tr>
	<tr>
		<td>Help Text</td>
		<td>fhelp</td>
		<td>->help('help text')</td>
	</tr>
	<tr>
		<td>Actions</td>
		<td>fa</td>
		<td>{{ Former::actions()->small_primary_submit('button') }}</td>
	</tr>
	</table>